<div align="center">

# GrowthOS AI

### The Execution Layer for Revenue Workflows

**10 specialized AI agents that research, qualify, score, approve, outreach, update CRM, and measure — orchestrated by workflows, governed by humans, visible end-to-end.**

[![License: Proprietary](https://img.shields.io/badge/License-Enterprise_Proprietary-blue.svg)](#license)
[![Status](https://img.shields.io/badge/Status-RC.5-green.svg)](#current-status)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB.svg)](https://python.org)
[![Next.js](https://img.shields.io/badge/Next.js-16-000000.svg)](https://nextjs.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.139-009688.svg)](https://fastapi.tiangolo.com)

</div>

---

## What GrowthOS AI Does

Revenue teams use 6-12 tools to move a lead from first touch to closed deal. CRM for records. Outreach for sequences. A separate tool for scoring. Another for research. Slack threads for handoffs. Spreadsheets for reporting. Nothing runs autonomously. Nothing connects.

**GrowthOS AI replaces this with a single execution layer.**

When a lead enters GrowthOS, AI agents automatically research the company, score the lead, qualify the prospect, draft outreach, update the CRM, and report on performance — with human approval at every high-risk step.

This is not another CRM. Not another outbound tool. Not another AI chatbot.

**It is an autonomous revenue workflow platform** — agents execute the work, workflows orchestrate the sequence, humans provide strategic oversight, and every action is measured.

---

## From Lead to Revenue

Here is what happens when a lead enters GrowthOS AI:

```
  Marketing / Lead Source
          |
          v
  +-----------------+
  |   LEAD INGEST   |   Web forms, CSV, API, LinkedIn, email
  +-----------------+   Leads enter the system from any channel
          |
          v
  +-----------------+
  | RESEARCH AGENT  |   Enriches lead with company data, tech stack,
  +-----------------+   news, intent signals, and organizational context
          |
          v
  +-------------------+
  | QUALIFICATION     |   Automated discovery: budget, authority,
  +-------------------+   need, timeline — structured qualification
          |
          v
  +-------------------+
  | LEAD SCORING      |   Custom criteria + historical patterns
  +-------------------+   produce a confidence-scored lead rank
          |
          v
     +---------+
     |DECISION |
     +----+----+
          |
    +-----+------+
    |            |
    v            v
  DISCARD    QUALIFIED
                |
                v
  +-------------------+
  | HUMAN APPROVAL    |   High-risk or high-value leads pause
  +-------------------+   for human review before proceeding
                |
                v
  +-------------------+
  | WORKFLOW ENGINE   |   DAG-based execution routes the lead
  +-------------------+   through the next steps in parallel or sequence
         |        |
         v        v
  +---------+  +-------------------+
  |   CRM   |  |    OUTREACH       |
  | UPDATE  |  |  Email / LinkedIn  |
  +---------+  |  WhatsApp / SMS    |
               +-------------------+
                         |
                         v
               +-------------------+
               | MEETING / PIPELINE|   Qualified leads convert
               +-------------------+   to pipeline opportunities
                         |
                         v
               +-------------------+
               | ANALYTICS + COST  |   Every step is measured:
               | + AUDIT           |   time, cost, outcome, agent
               +-------------------+   performance, full audit trail
```

**Every step has a WHY:**

| Step | What Happens | Why It Matters |
|------|-------------|----------------|
| Lead Ingest | Leads enter from any source | No lead is lost between tools |
| Research | Agent enriches with company data | Reps start with context, not空白 |
| Qualification | Structured discovery (BANT) | Consistent qualification criteria |
| Scoring | AI-ranked lead confidence | Sales focuses on highest-value leads |
| Human Approval | High-risk actions pause for review | Humans stay in control of critical decisions |
| Workflow Engine | Parallel and sequential execution | Complex processes run deterministically |
| CRM Update | Records stay current automatically | No manual data entry, no stale pipeline |
| Outreach | Multi-channel, context-aware | Right message, right channel, right timing |
| Analytics | Cost, time, outcome attribution | Know what works and what costs too much |

---

## The Operating Loop

GrowthOS AI runs as a closed-loop system. Every revenue workflow follows seven phases:

```
  +--------+    +------------+    +---------+    +----------------+
  | SENSE  |--->| UNDERSTAND |--->| DECIDE  |--->| ASK (if needed)|
  +--------+    +------------+    +---------+    +----------------+
                                                     |
  +--------+    +------------+    +---------+        |
  | LEARN  |<---|  MEASURE   |<---|  ACT    |<-------+
  +--------+    +------------+    +---------+
```

1. **Sense** — Detect incoming leads, signals, or triggers from any source
2. **Understand** — Research agents enrich with company data, intent signals, and context
3. **Decide** — Scoring and qualification agents determine priority and path
4. **Ask** — High-risk or high-value decisions pause for human approval
5. **Act** — Workflow engine executes outreach, CRM updates, and follow-ups
6. **Measure** — Every action, cost, and outcome is tracked in real time
7. **Learn** — Performance data feeds back into scoring models and workflow optimization

This loop runs continuously. The more it runs, the more data it collects, the smarter the decisions become.

**This is the core concept: not a set of disconnected tools, but a self-improving revenue execution system.**

---

## Why Not Just a CRM?

| Category | Primary Job | Limitation |
|----------|------------|------------|
| **CRM** | Store customer records | System of record; does not execute work |
| **Outbound Automation** | Send sequences at scale | Single-channel; no intelligence layer |
| **AI SDR** | Automate prospecting | Point solution; no workflow orchestration |
| **Workflow Automation** | Connect tools with rules | Generic; no domain-specific agents |
| **GrowthOS AI** | Orchestrate governed revenue workflows | Agents + workflows + approval + CRM + knowledge + observability |

Tools automate individual activities.

**GrowthOS orchestrates the entire governed revenue workflow.**

A CRM tells you what happened. An outbound tool sends what you tell it. An AI SDR chats with prospects. Workflow automation connects scripts.

GrowthOS does something none of these do: it takes a lead from ingestion through research, qualification, scoring, approval, outreach, CRM update, and measurement — as one coordinated, auditable, cost-tracked workflow with specialized AI agents at every step.

---

## What Makes GrowthOS Different

### 1. Revenue Workflow Orchestration
Not a lead list. Not a sequence builder. A complete lead-to-revenue workflow with branching, retries, dead letter queues, and checkpointing.

### 2. Multi-Agent Execution
10 specialized AI agents collaborate on complex workflows. Research, scoring, qualification, approval, CRM, outreach, proposals, analytics, human review, and supervisor — each agent has defined responsibilities, guardrails, and tool access.

### 3. Governed Autonomy
High-risk actions pause for human approval. Confidence thresholds trigger review. Risk classification determines the level of oversight. Speed of automation with judgment where it matters.

### 4. Context-Aware Execution
A built-in knowledge base (RAG) provides business-specific context to agents. Agents don't just follow rules — they access institutional knowledge to make better decisions.

### 5. Full Execution Visibility
Every workflow step, agent action, token cost, and approval decision is logged, traced, and attributed. Know exactly what happened, when, why, and what it cost.

### 6. SaaS-Ready Control Plane
Multi-tenant isolation, RBAC with 7 roles, tool authorization boundaries, idempotent operations, and emergency kill switch. Security and governance are part of the runtime, not bolted on.

---

## Why Customers Pay

### Today (Without GrowthOS)
- 6-12 disconnected tools
- Manual lead handoffs between systems
- Slow response times (hours or days)
- Inconsistent qualification criteria
- No visibility into cost per lead or workflow
- Reps doing coordination work instead of selling

### With GrowthOS
- One coordinated workflow
- AI agents execute research, qualification, scoring, outreach
- Faster response (minutes, not hours)
- Consistent, auditable qualification
- Human oversight at high-risk steps
- Measurable cost per workflow
- Reps focused on closing, not coordinating

**The value proposition is simple:** replace operational fragmentation with coordinated AI execution, and get measurable visibility into what each workflow costs and produces.

---

## Initial Wedge

### Who We Sell To First
Mid-market B2B companies (50-500 employees) with growing lead volume and fragmented revenue operations.

**Why this wedge:**
- Have outgrown basic CRM but cannot afford enterprise RevOps teams
- Already using 4-8 tools for lead management
- Feel the pain of manual handoffs and slow response
- Want automation but need governance and control

### The First Workflow
```
Lead Ingest -> Research -> Qualify -> Score -> Approve -> CRM -> Outreach -> Meeting
```

This is the highest-value, most universal revenue workflow. It is narrow enough to sell as a focused solution while using the full platform foundation.

Once this workflow is running, the same agents, engine, and governance layer can power additional workflows without rebuilding the core.

---

## Why This Can Become a Platform

### Initial Wedge
Lead / sales qualification workflow

### Adjacent Workflows (Same Platform)
- Lead reactivation (dormant pipeline)
- Merchant / partner acquisition
- Customer onboarding automation
- Revenue recovery (churn prevention)
- Campaign optimization loops
- Any workflow where AI agents execute governed revenue tasks

### What Stays the Same
- Agent runtime and lifecycle
- Workflow engine (DAG, retries, checkpoints)
- Tool authorization and risk classification
- Knowledge base and RAG
- Governance (approval gates, RBAC, audit)
- Observability (metrics, tracing, cost attribution)
- Multi-tenant SaaS control plane

**The platform thesis:** One agent runtime + one workflow engine + one governance layer = multiple revenue workflows on a single operating system.

---

## Architecture

```
+------------------------------------------------------------------+
|                     GROWTHOS AI PLATFORM                          |
+------------------------------------------------------------------+
|                                                                    |
|  +------------------------------------------------------------+  |
|  |                   WEB UI (Next.js 16)                       |  |
|  |  Dashboard - AI Workforce - Workflows - CRM - Analytics    |  |
|  +----------------------------+-------------------------------+  |
|                               | REST API                         |
|  +----------------------------v-------------------------------+  |
|  |                  API LAYER (FastAPI)                        |  |
|  |  Auth - Rate Limiting - RBAC - Tenant Isolation           |  |
|  +----------------------------+-------------------------------+  |
|                               |                                   |
|  +----------------------------v-------------------------------+  |
|  |               ORCHESTRATION ENGINE                          |  |
|  |  +----------+ +----------+ +----------+ +----------+      |  |
|  |  | Workflow | |  Agent   | | Approval | |  Tool    |      |  |
|  |  |  Engine  | | Runtime  | | Gateway  | | Executor |      |  |
|  |  +----------+ +----------+ +----------+ +----------+      |  |
|  +----------------------------+-------------------------------+  |
|                               |                                   |
|  +----------------------------v-------------------------------+  |
|  |              10 SPECIALIZED AI AGENTS                       |  |
|  |                                                              |  |
|  |  +---------+ +---------+ +---------+ +---------+           |  |
|  |  |Research | |  Lead   | |  Lead   | |Approval |           |  |
|  |  | Agent   | |Scoring  | |Qualifi- | | Agent   |           |  |
|  |  |         | | Agent   | | cation  | |         |           |  |
|  |  +---------+ +---------+ +---------+ +---------+           |  |
|  |  +---------+ +---------+ +---------+ +---------+           |  |
|  |  | Sales   | |  CRM    | |Proposal | |Analytics|           |  |
|  |  | Agent   | | Agent   | | Agent   | | Agent   |           |  |
|  |  +---------+ +---------+ +---------+ +---------+           |  |
|  |  +---------+ +-----------+                                 |  |
|  |  | Human   | | Supervisor|                                 |  |
|  |  | Review  | | Agent     |                                 |  |
|  |  +---------+ +-----------+                                 |  |
|  +----------------------------+-------------------------------+  |
|                               |                                   |
|  +----------------------------v-------------------------------+  |
|  |                     DATA LAYER                               |  |
|  |  PostgreSQL - Redis - Vector Store (RAG) - File Storage    |  |
|  +------------------------------------------------------------+  |
|                                                                    |
|  +------------------------------------------------------------+  |
|  |                   OBSERVABILITY                              |  |
|  |  Structured Logging - Prometheus Metrics - OpenTelemetry   |  |
|  +------------------------------------------------------------+  |
+------------------------------------------------------------------+
```

---

## AI Agents

GrowthOS ships with **10 specialized AI agents**, each purpose-built for a revenue operations function:

| Agent | Function | Status |
|-------|----------|--------|
| **Research Agent** | Enriches leads with company data, tech stack, news, and intent signals | Implemented |
| **Lead Scoring Agent** | Scores leads using custom criteria and historical patterns | Implemented |
| **Qualification Agent** | Runs automated discovery and qualifies prospects | Implemented |
| **Sales Agent** | Manages outbound sequences and handles objections | Implemented |
| **CRM Agent** | Keeps CRM records fresh with auto-updates and activity logging | Implemented |
| **Proposal Agent** | Generates custom proposals based on prospect requirements | Implemented |
| **Approval Agent** | Routes high-risk actions through human review before execution | Implemented |
| **Analytics Agent** | Generates insights, forecasts, and performance reports | Implemented |
| **Human Review Agent** | Handles escalated cases requiring human judgment and complex reasoning | Implemented |
| **Supervisor Agent** | Coordinates multi-agent workflows, monitors execution, and manages agent handoffs | Implemented |

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
- **RBAC** — Role-based access control with 7 roles (Super Admin, Org Admin, Workspace Admin, Manager, Operator, Viewer, API User) and granular permissions
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

## Screenshots

> Screenshots from the premium UI — live product captures coming soon.

| Screen | Preview |
|--------|---------|
| **Dashboard** | [SCREENSHOT: Dashboard with real-time agent fleet status and pipeline metrics] |
| **AI Workforce** | [SCREENSHOT: Visual agent grid with status, model, token usage, cost] |
| **Workflow Execution** | [SCREENSHOT: DAG visualization with step-by-step execution timeline] |
| **Approval Queue** | [SCREENSHOT: Pending approvals with confidence scores and full context] |
| **Lead Pipeline** | [SCREENSHOT: Lead list with AI scores, stages, and activity history] |
| **Analytics** | [SCREENSHOT: Executive KPI dashboard with cost attribution and forecasts] |

---

## Demo

> Live demo and video walkthrough coming soon.

### 01 — Dashboard
**What you see:** Real-time agent fleet status, lead pipeline metrics, system health, campaign overview
**What the system is doing:** Aggregating data from all agents, workflows, and CRM into a single operational view
**Why it matters:** One screen replaces 6 dashboards across separate tools

### 02 — Lead Ingestion
**What you see:** Leads entering from multiple sources (web forms, CSV, API, LinkedIn)
**What the system is doing:** Normalizing, validating, and routing incoming leads into the workflow engine
**Why it matters:** No lead falls through the cracks between tools

### 03 — AI Research
**What you see:** Research agent enriching a lead with company data, tech stack, news, intent signals
**What the system is doing:** Querying public data sources, company databases, and news feeds to build context
**Why it matters:** Reps start conversations with context, not guesses

### 04 — Qualification + Score
**What you see:** Qualification agent running discovery questions, scoring agent ranking the lead
**What the system is doing:** Applying BANT criteria and historical patterns to produce a structured qualification and confidence score
**Why it matters:** Consistent, objective qualification across all leads

### 05 — Workflow Timeline
**What you see:** Visual DAG with step-by-step execution, timing, and status
**What the system is doing:** Orchestrating parallel and sequential steps through the workflow engine
**Why it matters:** Complex processes run deterministically and are fully auditable

### 06 — Human Approval
**What you see:** Approval queue with confidence scores, risk levels, and full context
**What the system is doing:** Pausing high-risk actions and routing to designated reviewers
**Why it matters:** Humans stay in control of critical decisions

### 07 — Outreach + CRM
**What you see:** Multi-channel outreach (email, LinkedIn, WhatsApp, SMS) and CRM updates
**What the system is doing:** Executing context-aware outreach and keeping records current automatically
**Why it matters:** Right message, right channel, right timing — without manual data entry

### 08 — Analytics + Cost
**What you see:** Executive KPIs, cost attribution per agent/workflow, ROI metrics
**What the system is doing:** Aggregating performance data across all workflows and agents
**Why it matters:** Know exactly what each workflow costs and what it produces

### 09 — Audit / Governance
**What you see:** Complete audit trail of every action, decision, and approval
**What the system is doing:** Logging all operations with correlation IDs, timestamps, and actor context
**Why it matters:** Full traceability for compliance, debugging, and optimization

> **[LIVE DEMO URL]** | **[VIDEO URL]** | **[SCREENSHOTS]**

---

## For Investors

### Why Now

Three forces are converging:

1. **LLM and agent capabilities are becoming operationally useful** — AI agents can now execute multi-step business workflows reliably, not just answer questions
2. **Revenue teams already have fragmented software** — The average B2B sales stack includes 6-12 disconnected tools; coordination is the bottleneck
3. **Businesses want automation with control** — Full autonomy is risky; governed automation with human oversight is what enterprises actually need

The market is ready for a platform that orchestrates AI agents across revenue workflows with governance, visibility, and measurability built in.

### Why This Product

GrowthOS AI is a full-stack autonomous revenue workflow platform:

- **Agent runtime** with specialized agents, guardrails, and tool authorization
- **Workflow engine** with DAG execution, retries, checkpoints, and dead letter queues
- **Governance layer** with approval gates, risk classification, and confidence thresholds
- **Built-in CRM** with pipeline management and activity tracking
- **Knowledge base (RAG)** with tenant-scoped embeddings and semantic search
- **Observability** with Prometheus metrics, OpenTelemetry tracing, and cost attribution
- **Multi-tenant SaaS** with isolation, RBAC, and per-tenant quotas
- **Security** with fail-closed authorization, idempotent operations, and audit logging

This is not a prototype. It is a complete platform with 72 frontend pages, 80+ backend API endpoints, 10 AI agents, and a full observability stack.

### Why It Can Scale

The same platform foundation powers multiple revenue workflows:

- **Initial wedge:** Lead qualification and sales workflow
- **Adjacent workflows:** Lead reactivation, partner acquisition, customer onboarding, revenue recovery, campaign optimization
- **Reusable core:** Agent runtime, workflow engine, tool layer, governance, observability, multi-tenant control plane

Each new workflow uses the same agents, engine, and governance — just different configuration. The platform gets more valuable as more workflows are added.

### Market Positioning

GrowthOS AI sits at the intersection of three categories:

1. **CRM** (system of record) — GrowthOS includes a built-in CRM
2. **Sales automation** (execution layer) — GrowthOS orchestrates multi-channel outreach
3. **AI agents** (intelligence layer) — GrowthOS runs specialized agents with governance

**The thesis:** The future of revenue operations is not better tools — it is autonomous agents that execute governed workflows end-to-end. GrowthOS AI is the operating system for that future.

### Initial Customer Wedge

Mid-market B2B companies (50-500 employees) with growing lead volume and fragmented revenue operations:

- Have outgrown basic CRM but cannot afford enterprise RevOps teams
- Already using 4-8 tools for lead management
- Feel the pain of manual handoffs and slow response times
- Want automation but need governance and control

**First workflow:** Lead Ingest -> Research -> Qualify -> Score -> Approve -> CRM -> Outreach -> Meeting

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
