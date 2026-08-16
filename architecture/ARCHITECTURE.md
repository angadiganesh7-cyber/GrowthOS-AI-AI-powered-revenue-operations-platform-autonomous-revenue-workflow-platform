# GrowthOS AI — Architecture Overview

## System Design Principles

1. **Agent-first** — Every business function is modeled as an autonomous agent with defined inputs, outputs, and guardrails
2. **Tenant-isolated** — Multi-tenancy is a first-class concern, not an afterthought
3. **Fail-closed** — Security and authorization default to deny; actions require explicit permission
4. **Observable** — Every action is logged, traced, and metered
5. **Extensible** — New agents, tools, and workflows can be added without modifying core systems

---

## Core Components

### API Layer
- FastAPI with automatic OpenAPI documentation
- JWT-based authentication with refresh token rotation
- Rate limiting (Redis sliding-window with memory fallback)
- Request logging with correlation IDs

### Orchestration Engine
- DAG-based workflow execution
- Agent runtime with session management
- Tool authorization and risk classification
- Checkpointing and dead letter queues

### Agent Framework
- Base agent class with lifecycle hooks
- Input/output guardrails
- Memory management (short-term and long-term)
- Streaming support for real-time updates

### Data Layer
- PostgreSQL for persistent storage
- Redis for caching, rate limiting, and queues
- Vector embeddings for RAG
- File storage for documents and assets

### Observability
- Structured JSON logging
- Prometheus metrics
- OpenTelemetry distributed tracing
- Grafana dashboards

---

## Data Model (Simplified)

```
Organization
├── Workspace
│   ├── User (with role: ADMIN/MANAGER/USER)
│   ├── Agent (8 specialized types)
│   ├── Workflow (DAG definition)
│   │   └── WorkflowExecution
│   │       └── WorkflowStepExecution
│   ├── Lead
│   │   └── LeadScore
│   ├── Contact
│   ├── Company
│   ├── Deal
│   ├── Campaign
│   ├── Conversation
│   │   └── ConversationMessage
│   ├── KnowledgeBase
│   │   └── KnowledgeDocument
│   ├── ApprovalRequest
│   ├── ApiKey (hashed)
│   ├── Webhook
│   └── AuditLog
└── Subscription
    └── Invoice
```

---

## Security Architecture

```
Request → Rate Limiter → Auth Middleware → RBAC Check → Tenant Scope → Handler
                ↓                ↓              ↓            ↓
            Redis/DB         JWT Verify    Permission    Query Filter
            Sliding Window   Token Revoc.  Evaluation    Cross-Tenant
                                                          Block + Log
```

**Key security properties:**
- All secrets loaded from environment variables (never hardcoded)
- API keys stored as SHA-256 hashes
- Webhook payloads verified with HMAC-SHA256
- Tenant isolation enforced at the query level
- Cross-tenant access attempts are logged and blocked
- Tool execution requires explicit authorization
- AI outputs are filtered for PII before delivery
