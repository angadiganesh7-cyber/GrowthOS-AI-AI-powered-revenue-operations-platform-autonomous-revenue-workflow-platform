<div align="center">

# GrowthOS AI

### Autonomous Revenue Workflow Platform

**8 specialized AI agents. Real-time pipeline orchestration. Human-in-the-loop guardrails.**

[![License: Proprietary](https://img.shields.io/badge/License-Enterprise_Proprietary-blue.svg)](#license)
[![Status](https://img.shields.io/badge/Status-RC.5-green.svg)](#current-status)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB.svg)](https://python.org)
[![Next.js](https://img.shields.io/badge/Next.js-16-000000.svg)](https://nextjs.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.139-009688.svg)](https://fastapi.tiangolo.com)

</div>

---

## Problem

Revenue operations teams are drowning in tool fragmentation.

A typical B2B sales stack includes a CRM, an outbound automation tool, a lead scoring platform, an email sequencing tool, a workflow automation tool, a knowledge base, analytics dashboards, and approval systems. Each requires manual configuration, data stays siloed, and nothing runs autonomously.

**The result:** 12+ tabs open, 6+ integrations to maintain, and humans doing the coordination work that software should handle.

GrowthOS AI replaces this fragmented stack with a single autonomous platform where AI agents handle the operational work end-to-end, with humans providing strategic oversight.

---

## What GrowthOS AI Is

GrowthOS AI is an **autonomous revenue workflow platform** — a multi-agent AI operating system that:

- **Ingests** leads from any source (web forms, CSV, API, LinkedIn, email)
- **Researches** companies and contacts using real-time data
- **Scores** leads using custom criteria and AI-powered analysis
- **Qualifies** prospects through automated discovery
- **Nurtures** relationships across email, LinkedIn, WhatsApp, SMS, and voice
- **Proposes** solutions with AI-generated proposals
- **Approves** high-risk actions through configurable human-in-the-loop workflows
- **Tracks** everything in a built-in CRM with pipeline visibility
- **Reports** on performance with real-time analytics and cost attribution

All orchestrated through a **visual workflow engine** with DAG-based execution, retry policies, and distributed tracing.

---

## Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                    GROWTHOS AI PLATFORM                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                    WEB UI (Next.js 16)                  │   │
│  │  Dashboard · AI Workforce · Workflows · CRM · Analytics │   │
│  └────────────────────────┬────────────────────────────────┘   │
│                           │ REST API                            │
│  ┌────────────────────────▼────────────────────────────────┐   │
│  │                  API LAYER (FastAPI)                     │   │
│  │  Auth · Rate Limiting · RBAC · Tenant Isolation         │   │
│  └────────────────────────┬────────────────────────────────┘   │
│                           │                                     │
│  ┌────────────────────────▼────────────────────────────────┐   │
│  │              ORCHESTRATION ENGINE                        │   │
│  │  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐  │   │
│  │  │ Workflow  │ │  Agent   │ │ Approval │ │  Tool    │  │   │
│  │  │  Engine   │ │ Runtime  │ │ Gateway  │ │Executor  │  │   │
│  │  └──────────┘ └──────────┘ └──────────┘ └──────────┘  │   │
│  └────────────────────────┬────────────────────────────────┘   │
│                           │                                     │
│  ┌────────────────────────▼────────────────────────────────┐   │
│  │              8 SPECIALIZED AI AGENTS                     │   │
│  │                                                           │   │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐       │   │
│  │  │Research │ │  Lead   │ │  Lead   │ │Approval │       │   │
│  │  │ Agent   │ │Scoring  │ │Qualifi- │ │ Agent   │       │   │
│  │  │         │ │ Agent   │ │ cation  │ │         │       │   │
│  │  └─────────┘ └─────────┘ └─────────┘ └─────────┘       │   │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐       │   │
│  │  │ Sales   │ │  CRM    │ │Proposal │ │Analytics│       │   │
│  │  │ Agent   │ │ Agent   │ │ Agent   │ │ Agent   │       │   │
│  │  └─────────┘ └─────────┘ └─────────┘ └─────────┘       │   │
│  └────────────────────────┬────────────────────────────────┘   │
│                           │                                     │
│  ┌────────────────────────▼────────────────────────────────┐   │
│  │                    DATA LAYER                            │   │
│  │  PostgreSQL · Redis · Vector Store (RAG) · File Storage  │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                 OBSERVABILITY                            │   │
│  │  Structured Logging · Prometheus Metrics · OpenTelemetry │   │
│  └─────────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────────┘
```

---

## AI Agents

GrowthOS ships with **8 specialized AI agents**, each purpose-built for a revenue operations function:

| Agent | Function | Status |
|-------|----------|--------|
| **Research Agent** | Enriches leads with company data, tech stack, news, and intent signals | Implemented |
| **Lead Scoring Agent** | Scores leads using custom criteria and historical patterns | Implemented |
| **Qualification Agent** | Runs automated discovery calls and qualifies prospects | Implemented |
| **Sales Agent** | Manages outbound sequences and handles objections | Implemented |
| **CRM Agent** | Keeps CRM records fresh with auto-updates and activity logging | Implemented |
| **Proposal Agent** | Generates custom proposals based on prospect requirements | Implemented |
| **Approval Agent** | Routes high-risk actions through human review before execution | Implemented |
| **Analytics Agent** | Generates insights, forecasts, and performance reports | Implemented |

Each agent operates within a **sandboxed execution environment** with:
- Input guardrails (prompt injection detection)
- Output guardrails (PII filtering)
- Risk classification (low/medium/high/critical)
- Tool authorization boundaries
- Token budget enforcement

---

## Human-in-the-Loop

Not every action should be fully autonomous. GrowthOS provides configurable human oversight at every level:

- **Approval workflows** — Critical actions (sending proposals, large contracts, data deletion) route to designated reviewers before execution
- **Risk classification** — Tools and actions are classified by risk level; higher-risk actions require human sign-off
- **Confidence thresholds** — When agent confidence falls below a configurable threshold, the system pauses for human review
- **Audit trail** — Every action, decision, and approval is logged with full traceability

This means you get the speed of automation with the judgment of human oversight where it matters.

---

## Workflow Orchestration

The visual workflow engine enables complex multi-step revenue processes:

- **DAG-based execution** — Define workflows as directed acyclic graphs with parallel and sequential steps
- **Conditional branching** — Route leads through different paths based on score, industry, company size, or custom logic
- **Retry policies** — Configurable retry with exponential backoff for transient failures
- **Dead letter queues** — Failed executions are captured for inspection and replay
- **Checkpointing** — Long-running workflows can pause and resume across sessions
- **Event-driven triggers** — Workflows can be triggered by API calls, webhooks, schedules, or other workflow completions

**Example workflow:**
```
Lead Ingested → Research → Score → Qualify → Route to Sales → Send Proposal → Await Approval → Execute
```

---

## RAG / Knowledge Base

Agents access institutional knowledge through a built-in RAG (Retrieval-Augmented Generation) system:

- **Vector store** with tenant-scoped embeddings
- **Document ingestion** from PDFs, URLs, and structured data
- **Semantic search** across the knowledge base
- **Context injection** — Relevant knowledge is automatically retrieved and injected into agent prompts
- **Freshness controls** — Knowledge base entries can be versioned and expired

---

## Observability

You can't improve what you can't measure. GrowthOS provides full-stack observability:

- **Structured JSON logging** with correlation IDs across requests and agent executions
- **Prometheus metrics** — Request rates, latencies, agent execution counts, token usage, cost attribution
- **Distributed tracing** — OpenTelemetry-compatible traces across workflow steps
- **Real-time dashboards** — Agent health, pipeline metrics, cost analytics, and performance benchmarks
- **Alerting** — Configurable alerts for error rates, latency thresholds, and budget limits

---

## Security Approach

Security is foundational, not an afterthought:

- **Multi-tenant isolation** — Row-level security with organization-scoped data access; cross-tenant queries are blocked and logged
- **JWT authentication** — Access + refresh token rotation with JTI-based revocation
- **RBAC** — Role-based access control with 5 roles (Super Admin, Admin, Manager, User, API User) and granular permissions
- **Rate limiting** — Redis sliding-window rate limiter with stricter limits on auth endpoints
- **Account lockout** — 5 failed attempts triggers 15-minute lockout
- **Password policy** — OWASP-compliant complexity requirements
- **Security headers** — CSP, HSTS, X-Frame-Options, and other OWASP-recommended headers
- **API key security** — SHA-256 hashed storage, never stored raw
- **Webhook verification** — HMAC-SHA256 signature verification on all incoming webhooks
- **AI guardrails** — Prompt injection detection, output PII filtering, tool execution policies
- **Kill switch** — Emergency maintenance mode to halt all write operations
- **Audit logging** — Complete audit trail of all administrative and data access actions

---

## Technology Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | Next.js 16 (App Router), React 19, TypeScript, TailwindCSS v4, Framer Motion |
| **Backend** | Python 3.11+, FastAPI 0.139, SQLAlchemy 2.0, Alembic |
| **Database** | PostgreSQL (production), SQLite (development) |
| **Cache / Queue** | Redis |
| **AI Providers** | Google Gemini, OpenRouter (multi-model gateway), OpenAI, Anthropic, Ollama (local) |
| **Vector Store** | Embedded vector search for RAG |
| **Observability** | Prometheus, Grafana, OpenTelemetry |
| **Auth** | JWT (HS256), bcrypt, OAuth2 (Google/GitHub), OIDC, SAML 2.0 (stubs) |
| **Billing** | Stripe, Razorpay (mock integrations) |
| **Deployment** | Docker, Kubernetes, Helm |
| **CI/CD** | GitHub Actions (pytest, Bandit, Trivy, Docker build) |

---

## Current Status

**Version:** RC.5 (Release Candidate 5)

| Capability | Status |
|------------|--------|
| Multi-agent orchestration | Implemented |
| Visual workflow engine | Implemented |
| CRM with pipeline management | Implemented |
| Lead ingestion and management | Implemented |
| Email/LinkedIn/WhatsApp/SMS communication | Implemented |
| Human-in-the-loop approvals | Implemented |
| Multi-tenant SaaS platform | Implemented |
| Billing and subscription management | Implemented |
| RBAC and audit logging | Implemented |
| Analytics and reporting | Implemented |
| Knowledge base (RAG) | Implemented |
| AI guardrails and security | Implemented |
| Observability (metrics, logging, tracing) | Implemented |
| Production deployment (Kubernetes) | Implemented |
| Agent marketplace | Partial |
| Voice calls | Partial |
| Industry-specific templates | Partial |

---

## Roadmap

See [roadmap/ROADMAP.md](roadmap/ROADMAP.md) for the detailed product roadmap.

**Near-term priorities:**
- Production hardening and performance optimization
- Enhanced agent collaboration patterns
- Deeper CRM integrations (Salesforce, HubSpot)
- Advanced analytics and forecasting
- Agent marketplace and custom agent builder

---

## Demo

> Live demo and video walkthrough coming soon.

**What the demo shows:**
1. Dashboard with real-time agent fleet status
2. Lead ingestion and automated research
3. AI-powered lead scoring and qualification
4. Workflow execution with visual timeline
5. Human approval flow
6. Multi-channel outreach (email, LinkedIn)
7. Analytics and cost attribution

---

## For Investors

GrowthOS AI is positioned at the intersection of three massive markets:

1. **CRM ($80B+)** — The systems of record for customer relationships
2. **Sales Automation ($30B+)** — The tools that execute revenue workflows
3. **AI Agents ($50B+ by 2028)** — The autonomous systems that replace manual operations

**Our thesis:** The future of revenue operations is not better tools — it's autonomous agents that operate the tools for you. GrowthOS AI is the operating system for that future.

**Initial wedge:** Mid-market B2B SaaS companies (50-500 employees) who have outgrown basic CRM but can't afford enterprise RevOps teams.

**Long-term platform:** An extensible agent marketplace where companies can deploy, compose, and share specialized AI agents for any revenue function.

---

## Founders

> *Founder section — to be completed with actual founder bios, photos, and contact information.*

---

## License

Proprietary — All rights reserved.

This repository is provided for investor review purposes only. Unauthorized copying, distribution, or use is prohibited.

---

<div align="center">

**[Request Demo](mailto:demo@growthos.ai)** · **[Documentation](docs/)** · **[Architecture](architecture/)**

</div>
