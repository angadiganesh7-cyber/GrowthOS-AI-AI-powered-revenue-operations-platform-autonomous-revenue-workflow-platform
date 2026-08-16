<div align="center">

# GrowthOS

### The AI Business Execution Platform

**GrowthOS AI — Revenue Operations** is the first application built on the GrowthOS platform.

**Lead in. Research. Qualify. Score. Approve. Outreach. CRM. Meeting. Measure.**
**One platform. 10 AI agents. Full workflow. Human oversight. Every action visible.**

[![License: Proprietary](https://img.shields.io/badge/License-Enterprise_Proprietary-blue.svg)](#license)
[![Status](https://img.shields.io/badge/Status-RC.5-green.svg)](#current-status)

</div>

---

## The Problem

Revenue operations teams run 6-12 disconnected tools to move a lead from first touch to closed deal. A CRM stores records. An enrichment tool researches companies. A scoring platform ranks leads. An outbound tool sends sequences. Slack handles handoffs. Spreadsheets track reporting. Nothing runs autonomously. Nothing connects.

**The cost of this fragmentation:**

| Pain Point | What Happens | Impact |
|------------|-------------|--------|
| Tool fragmentation | Multiple logins and integrations to maintain | Reps spend significant time on coordination instead of selling |
| Manual handoffs | Leads pass between tools via copy-paste or scripts | Response time drops from minutes to hours or days |
| Inconsistent qualification | Each rep qualifies differently | Pipeline quality varies; bad deals waste engineering time |
| No workflow visibility | No single view of the lead-to-meeting process | Cannot measure cost per lead or identify bottlenecks |
| No cost attribution | Token usage, API calls, and agent work are unmetered | Cannot determine which workflows produce ROI |

> **Source note:** The pain points above are based on commonly observed B2B revenue operations patterns. The "6-12 tools" figure reflects typical mid-market B2B sales stacks (CRM + enrichment + outbound + scoring + analytics + communication + workflow). No proprietary measurement data is cited.

**GrowthOS AI replaces this fragmentation with a single execution layer.**

---

## What GrowthOS AI Does

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

---

## Illustrative Lead Journey

> **This is an illustrative example, not a customer case study.** It shows how a lead would flow through the complete GrowthOS workflow.

**Scenario:** A 150-person B2B SaaS company receives a lead from a webinar signup.

| Step | What Happens | System Action |
|------|-------------|---------------|
| **1. Ingest** | Lead enters via webinar registration API | Normalized, de-duplicated, source attributed as "webinar" |
| **2. Research** | Research Agent enriches with company data | Finds: 150 employees, Series B, uses Salesforce + Outreach + ZoomInfo, recent funding announcement |
| **3. Qualify** | Qualification Agent runs BANT discovery | Budget: confirmed (recent fundraise). Authority: VP Marketing registered. Need: scaling outbound. Timeline: Q2. |
| **4. Score** | Scoring Agent ranks the lead | Score: 84/100. High intent, good fit, timing aligned. |
| **5. Decision** | Score exceeds threshold (70+) | Routed to qualified pipeline |
| **6. Approval** | Approval Agent flags for manager review | Confidence: 84%. Risk: Medium (new contact, no prior interaction). Pauses for human sign-off. |
| **7. Human Review** | Manager reviews in approval queue | Sees: company data, qualification, score, proposed outreach. Approves with one click. |
| **8. CRM Update** | CRM Agent creates contact + deal | Contact created, deal opened at $24K ARR, activity logged, source tagged |
| **9. Outreach** | Sales Agent drafts personalized email | References: recent fundraise, scaling outbound, uses 3 tools GrowthOS could replace |
| **10. Multi-channel** | Follow-up via LinkedIn + email sequence | Day 1: email. Day 3: LinkedIn connection. Day 5: follow-up email with case study. |
| **11. Pipeline** | Lead responds, meeting booked | Deal stage advances to "Discovery Scheduled." CRM updated automatically. |
| **12. Analytics** | Workflow metrics recorded | Time to meeting: 5 days. Cost: agent tokens + API calls. Source: webinar. |

**Total time from lead entry to meeting booked: 5 days.**

> These timelines are illustrative. Actual performance depends on lead quality, agent configuration, and human review speed.

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

> GrowthOS AI is the first application demonstrating this capability. The same platform foundation can orchestrate other business workflows.

---

## Why Not Salesforce + Zapier + LangChain?

An investor may ask: "Why can't a company just wire together Salesforce (CRM) + Zapier (automation) + LangChain or CrewAI (AI agents)?"

**They can. Here is why they would not want to.**

| Requirement | Salesforce + Zapier + LangChain | GrowthOS |
|-------------|--------------------------------|----------|
| Lead-to-meeting workflow | Build custom: Salesforce API + Zapier triggers + LangChain agent + custom approval logic | Built-in: complete lead-to-revenue workflow with 10 agents |
| Human approval gates | Custom code: build approval UI, webhook handlers, state management | Built-in: approval queue with confidence scores, risk levels, one-click approve/reject |
| Multi-agent coordination | Custom code: manage agent sessions, shared memory, handoffs | Built-in: 10 specialized agents with defined responsibilities and guardrails |
| Tool authorization | Custom code: build auth boundaries, risk classification per tool | Built-in: fail-closed `ToolExecutor.authorize()` with risk levels |
| Cost attribution | Custom code: track token usage, API costs, map to workflows | Built-in: per-agent, per-workflow, per-lead cost attribution |
| Multi-tenant SaaS | Custom code: build tenant isolation, RBAC, quotas from scratch | Built-in: organization-scoped isolation, 7 roles, per-tenant quotas |
| Observability | Custom code: instrument each service, build dashboards | Built-in: Prometheus metrics, OpenTelemetry tracing, structured logging |
| Maintenance | Update 3+ systems, manage integrations, fix breakages | Single platform, single deployment |

**The build-vs-buy tradeoff:**
- **Build:** Requires significant integration engineering. Ongoing maintenance of 3+ systems. Custom approval logic. Custom observability. Custom multi-tenancy.
- **Buy:** Complete platform, ready to configure. Governance, observability, and multi-tenancy included.

GrowthOS is not a framework. It is an integrated revenue-execution product layer combining orchestration, governance, observability, and workflow controls in one system.

---

## GrowthOS Ecosystem

```
              GROWTHOS
       AI Business Execution Platform
                   |
    Shared Runtime / Agents / Workflows
    Governance / Observability / Tenancy
                   |
     +-------------+-------------+
     |             |             |
     v             v             v
  GrowthOS AI   LogGlance AI   Future
  Revenue Ops   AI Operations  Applications
  [CURRENT]     [FUTURE]       [FUTURE]
```

GrowthOS is the **parent AI business execution platform**. It provides a shared execution and governance foundation on which multiple specialized business applications can operate.

**GrowthOS AI — Revenue Operations** is the first implemented application. It uses the full platform to execute the lead-to-revenue lifecycle with AI agents.

**LogGlance AI — Future Application Concept** is a planned future application concept within the GrowthOS ecosystem, focused on AI operations and observability. The concept is intended to address organizations operating AI-enabled software and business-critical systems. It has not yet been built, launched, or commercially validated.

**Future Applications** — The same platform foundation is designed to support additional business-operation workflows, including customer onboarding, revenue recovery, partner operations, and other AI-enabled business workflows. These are expansion opportunities, not currently built products.

### The GrowthOS Platform Thesis

GrowthOS is not intended to be a collection of unrelated SaaS products. The strategy is to build a reusable AI execution platform and launch focused applications on top of it. GrowthOS AI is the first wedge; additional applications expand the addressable market without rebuilding the underlying execution infrastructure.

The platform provides shared capabilities that every application inherits:

| Shared Capability | What It Provides |
|-------------------|-----------------|
| **AI Agent Runtime** | Multi-agent lifecycle, session management, context propagation |
| **Reusable Agents** | Specialized agents with defined responsibilities, guardrails, and tool access |
| **Workflow Engine** | DAG-based execution, retries, checkpoints, dead letter queues |
| **Human Approval Mechanisms** | Configurable approval gates, confidence thresholds, risk classification |
| **Tool Authorization** | Fail-closed tool boundaries, risk levels, per-agent tool access |
| **Observability & Cost Controls** | Prometheus metrics, OpenTelemetry tracing, per-action cost attribution |
| **Multi-Tenancy & RBAC** | Organization isolation, workspace scoping, 7-role permission hierarchy |
| **Auditability** | Complete audit trail with correlation IDs on every operation |
| **Integrations** | Pluggable tool layer for external APIs, CRMs, and data sources |

The pattern follows a **Shopify-like ecosystem model** — shared platform infrastructure on which multiple specialized applications operate. This is an analogy to explain the platform-and-applications architecture, not a direct comparison to Shopify as a company or market position.

### Why This Architecture Works

- **One execution infrastructure** — built once, reused across applications
- **One governance layer** — approval gates, RBAC, audit, cost attribution shared across all apps
- **One workflow engine** — DAG orchestration, retries, checkpoints for any business process
- **One agent runtime** — multi-agent coordination, tool authorization, guardrails for any domain
- **Multiple applications** — each addressing a distinct business problem with domain-specific agents and workflows

Each new application reuses the platform foundation. The platform gets more valuable as more applications are built on it.

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

### Today (Without GrowthOS AI)
- 6-12 disconnected tools
- Manual lead handoffs between systems
- Slow response times (hours or days)
- Inconsistent qualification criteria
- No visibility into cost per lead or workflow
- Reps doing coordination work instead of selling

### With GrowthOS AI
- One coordinated workflow
- AI agents execute research, qualification, scoring, outreach
- Faster response (minutes, not hours)
- Consistent, auditable qualification
- Human oversight at high-risk steps
- Measurable cost per workflow
- Reps focused on closing, not coordinating

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

---

## Why This Can Become a Platform

### Initial Wedge
GrowthOS AI — lead qualification and revenue operations workflow (shipped, RC.5)

### Second Application (Future Concept)
LogGlance AI — future application concept for AI operations / observability (not yet built)

### Adjacent Workflows (Same Platform)
- Lead reactivation (dormant pipeline)
- Partner / merchant acquisition
- Customer onboarding automation
- Revenue recovery (churn prevention)
- Campaign optimization loops
- Any workflow where AI agents execute governed business tasks

### What Stays the Same Across Applications
- Agent runtime and lifecycle
- Workflow engine (DAG, retries, checkpoints)
- Tool authorization and risk classification
- Governance (approval gates, RBAC, audit)
- Observability (metrics, tracing, cost attribution)
- Multi-tenant SaaS control plane

**The platform thesis:** One agent runtime + one workflow engine + one governance layer = multiple business applications on a single execution platform.

---

## Current Stage

| Attribute | Status |
|-----------|--------|
| **Product version** | RC.5 (Release Candidate 5) |
| **Product status** | Working product — 72 frontend pages, 191 API endpoints, 10 AI agents |
| **Validation stage** | Product validation / demo stage |
| **Customers** | None claimed. No production deployments yet. |
| **Revenue** | None claimed. No commercial transactions yet. |
| **Team** | Founder and team details will be presented in the Antler application |
| **Next milestones** | Demo deployment, design partner pilots, first revenue |

**What is built and verified:**
- Complete multi-agent orchestration runtime
- 10 specialized AI agents with guardrails
- DAG-based workflow engine with retries, checkpoints, dead letter queues
- Built-in CRM with pipeline management
- Human-in-the-loop approval system
- Multi-tenant SaaS with isolation, RBAC, and quotas
- AI guardrails (prompt injection detection, PII filtering)
- Observability (Prometheus, OpenTelemetry, structured logging)
- Idempotent operations across usage, cost, CRM, email, and approval
- Emergency kill switch
- 810/810 tests passing (internal testing, not production-validated)

> All metrics above are from internal testing and development, not production deployments. Production metrics will be tracked and reported after customer deployments.

---

## Business Model

> **Proposed model — not yet commercially validated.**

GrowthOS AI is intended to operate as a B2B SaaS platform with tiered subscription pricing.

| Dimension | Approach |
|-----------|----------|
| **Revenue model** | Monthly/annual SaaS subscription |
| **Pricing levers** | Number of agents, workflow volume, seats, features |
| **Target ACV** | Mid-market range (to be validated through customer discovery) |
| **Free tier** | Potential limited free tier for evaluation and product-led growth |
| **Enterprise tier** | Custom pricing for dedicated infrastructure, SLA, and support |

**Proposed tier structure:**

| Tier | Target | Include |
|------|--------|---------|
| **Starter** | Early-stage B2B, small teams | Core agents, limited workflow volume, community support |
| **Growth** | Mid-market B2B (50-200 employees) | Full agent suite, higher workflow volume, email support |
| **Enterprise** | Mid-market to upper-mid (200-500 employees) | Custom agents, unlimited workflows, dedicated support, SSO |

> Pricing specifics will be determined through customer discovery and market testing. The above is a framework, not a validated price list.

---

## Go-to-Market Strategy

> **Planned strategy — not yet executed.**

### Phase 1: Design Partners (Months 1-3)
- Recruit 5-10 design partners from mid-market B2B companies
- Offer free access in exchange for feedback and case studies
- Validate the lead qualification workflow with real leads
- Iterate on agent performance and workflow configuration

### Phase 2: Early Customers (Months 3-6)
- Convert best design partners to paying customers
- Founder-led sales to first 10-20 customers
- Target companies currently using 4+ tools for lead management
- Position as replacement for fragmented RevOps stack

### Phase 3: Scaling (Months 6-12)
- Content marketing: publish insights on revenue operations fragmentation
- Direct outreach to companies using Salesforce + Outreach + ZoomInfo stacks
- Partnerships with RevOps consultants and agencies
- Product-led growth tier for self-serve evaluation

### Customer Acquisition Channels
1. **Founder-led sales** — Direct outreach to target companies
2. **Content marketing** — Revenue operations thought leadership
3. **Community** — RevOps communities, LinkedIn, B2B SaaS forums
4. **Partnerships** — RevOps consultants, Salesforce consultants, agencies
5. **Product-led growth** — Free tier for evaluation and viral adoption

---

## Market Sizing

> **Methodology-based framework — not proprietary market research.** Specific dollar figures require validated industry reports. Below is the sizing approach we would use with verified data.

### Approach

Market sizing uses publicly available industry reports (Gartner, IDC, Forrester, Statista) and analyst estimates. Ranges reflect uncertainty in sub-segment definitions.

### TAM (Total Addressable Market)

The global market for CRM, sales automation, and AI agent platforms. We would source this from:
- **Global CRM market:** Gartner "Market Guide for CRM" or IDC "Worldwide CRM Software" reports
- **Sales engagement / outbound automation:** Gartner "Market Guide for Sales Engagement" or Forrester "Sales Automation Wave"
- **AI agents / intelligent automation:** Gartner "Market Guide for AI Trust, Risk and Security Management" or IDC "AI Agent Forecast"

> **Current status:** We have not yet purchased or verified specific report figures. TAM will be populated with sourced numbers after market research is completed.

### SAM (Serviceable Addressable Market)

Mid-market B2B companies (50-500 employees) with revenue operations teams:

- B2B companies in this employee range in North America and Europe (source: ZoomInfo, LinkedIn Sales Navigator market data — to be verified)
- Current spend on revenue tools per company (source: industry surveys — to be verified)
- **SAM will be calculated after verifying company counts and average tool spend through primary research**

### SOM (Serviceable Obtainable Market)

Initial wedge: mid-market B2B companies with 4+ revenue tools and growing lead volume:

- Subset of SAM with acute fragmentation pain
- Initial target: first 10-50 design partners and early customers in first 2-3 years
- **SOM will be estimated after design partner recruitment and initial customer discovery**

> These are directional placeholders. All market sizing will be populated with verified, sourced numbers before investor submission. We prioritize accuracy over impressive-looking figures.

---

## For Investors

### Why Now

Three forces are converging:

1. **LLM and agent capabilities are becoming operationally useful** — AI agents can now execute multi-step business workflows reliably, not just answer questions
2. **Revenue teams already have fragmented software** — The average B2B sales stack includes 6-12 disconnected tools; coordination is the bottleneck
3. **Businesses want automation with control** — Full autonomy is risky; governed automation with human oversight is what enterprises actually need

The market is ready for a platform that orchestrates AI agents across revenue workflows with governance, visibility, and measurability built in.

### Why This Problem

Revenue operations is the highest-cost, lowest-visibility function in B2B sales. Companies invest in multiple tools but cannot answer: "What does it cost to get a lead from first touch to meeting?" The tools do not connect. The data does not flow. The workflows do not coordinate.

### Why This Product

GrowthOS AI is a full-stack autonomous revenue workflow platform — the first application built on the GrowthOS shared AI business execution platform:

- **Agent runtime** with specialized agents, guardrails, and tool authorization
- **Workflow engine** with DAG execution, retries, checkpoints, and dead letter queues
- **Governance layer** with approval gates, risk classification, and confidence thresholds
- **Built-in CRM** with pipeline management and activity tracking
- **Knowledge base (RAG)** with tenant-scoped embeddings and semantic search
- **Observability** with Prometheus metrics, OpenTelemetry tracing, and cost attribution
- **Multi-tenant SaaS** with isolation, RBAC, and per-tenant quotas
- **Security** with fail-closed authorization, idempotent operations, and audit logging

This is not a prototype. It is a complete platform with 72 frontend pages, 191 backend API endpoints, 10 AI agents, and a full observability stack.

The platform foundation is designed to be reusable. LogGlance AI is one future application concept that could demonstrate this reusability — same platform, different application, different market. It has not yet been built.

### Why This Can Scale

The GrowthOS platform is designed to power multiple business applications:

- **Initial wedge:** GrowthOS AI — revenue operations (shipped, RC.5)
- **Future application concept:** LogGlance AI — AI operations / observability (not yet built)
- **Adjacent revenue workflows:** Lead reactivation, partner acquisition, customer onboarding, revenue recovery, campaign optimization
- **Cross-industry expansion:** Customer onboarding, revenue recovery, partner operations, and other AI-enabled business workflows (expansion opportunity)
- **Reusable core:** Agent runtime, workflow engine, tool layer, governance, observability, multi-tenant control plane

Each new application reuses the platform foundation. The platform gets more valuable as more applications are built on it.

### Investor Thesis

> **Initial wedge → reusable platform → multiple applications → cross-industry expansion**

1. **Wedge:** GrowthOS AI solves revenue operations fragmentation for mid-market B2B — a clear, acute pain point with existing demand
2. **Platform:** The same AI execution infrastructure (agent runtime, workflow engine, governance, observability) is reusable across business domains
3. **Future applications:** LogGlance AI is one future application concept that demonstrates the potential — same platform, different application, different market (not yet built)
4. **Cross-industry:** The platform is designed for expansion into additional business-operation workflows across industries

The strategic thesis: build the AI execution infrastructure once, then deploy multiple specialized business applications on top of it.

GrowthOS AI is the first implemented application and current product wedge. The longer-term vision is to reuse the underlying platform capabilities to support additional specialized applications. LogGlance AI is one future application concept, not a currently built product.

### Founder and Team

> Founder and team details, including domain expertise and relevant experience, will be presented in the Antler application.

---

## Architecture

```
+------------------------------------------------------------------+
|                     GROWTHOS                                      |
|              AI Business Execution Platform                       |
+------------------------------------------------------------------+
|                                                                    |
|  +------------------------------------------------------------+  |
|  |           SHARED EXECUTION + GOVERNANCE FOUNDATION          |  |
|  |                                                             |  |
|  |  +-------------+ +-------------+ +-------------+          |  |
|  |  |   Agent     | |  Workflow   | |  Approval   |          |  |
|  |  |   Runtime   | |  Engine     | |  Gateway    |          |  |
|  |  +-------------+ +-------------+ +-------------+          |  |
|  |  +-------------+ +-------------+ +-------------+          |  |
|  |  |    Tool     | |  Knowledge  | | Observabil. |          |  |
|  |  |  Executor   | |  Base (RAG) | | + Cost Attr |          |  |
|  |  +-------------+ +-------------+ +-------------+          |  |
|  |  +-------------+ +-------------+ +-------------+          |  |
|  |  | Multi-      | |    RBAC     | |   Audit     |          |  |
|  |  | Tenancy     | |  7 Roles    | |   Trail     |          |  |
|  |  +-------------+ +-------------+ +-------------+          |  |
|  +----------------------------+-------------------------------+  |
|                               |                                   |
|  +----------------------------v-------------------------------+  |
|  |                    APPLICATIONS                             |  |
|  |                                                             |  |
|  |  +-------------------+  +-------------------+             |  |
  |  |  |  GrowthOS AI      |  |  LogGlance AI     |             |  |
|  |  |  Revenue Ops      |  |  AI Operations    |             |  |
|  |  |  [CURRENT]        |  |  [FUTURE]         |             |  |
|  |  +-------------------+  +-------------------+             |  |
|  |                                                             |  |
|  |               +-------------------+                        |  |
|  |               | Future            |                        |  |
|  |               | Applications      |                        |  |
|  |               | [PLANNED]         |                        |  |
|  |               +-------------------+                        |  |
|  +------------------------------------------------------------+  |
|                                                                    |
|  +------------------------------------------------------------+  |
|  |                     DATA LAYER                               |  |
|  |  PostgreSQL - Redis - Vector Store (RAG) - File Storage    |  |
|  +------------------------------------------------------------+  |
+------------------------------------------------------------------+
```

---

## AI Agents

GrowthOS ships with **10 specialized AI agents**, each purpose-built for a revenue operations function:

| Agent | Function | Implementation Status |
|-------|----------|----------------------|
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
| **Billing** | Stripe, Razorpay (mock integrations for development) |
| **Deployment** | Docker, Kubernetes, Helm |
| **CI/CD** | GitHub Actions (pytest, Bandit, Trivy, Docker build) |

---

## Screenshots

> **Status: Placeholders — screenshots will be captured from the working product before investor submission.**

| Screen | Description | Status |
|--------|-------------|--------|
| **Dashboard** | Real-time agent fleet status, lead pipeline metrics, system health | Planned |
| **AI Workforce** | Visual agent grid with status, model, token usage, cost | Planned |
| **Workflow Execution** | DAG visualization with step-by-step execution timeline | Planned |
| **Approval Queue** | Pending approvals with confidence scores and full context | Planned |
| **Lead Pipeline** | Lead list with AI scores, stages, and activity history | Planned |
| **Analytics** | Executive KPI dashboard with cost attribution and forecasts | Planned |

> Screenshots will be added to `screenshots/` directory from the premium UI.

---

## Demo

> **Status: Coming after demo validation.** Live demo and video walkthrough will be deployed before investor submission.

### What the Demo Shows

| Step | What You See | What the System Does |
|------|-------------|---------------------|
| **01 — Dashboard** | Agent fleet status, pipeline metrics, system health | Aggregates data from all agents and workflows |
| **02 — Lead Ingestion** | Leads entering from multiple sources | Normalizes, validates, routes into workflow engine |
| **03 — AI Research** | Research agent enriching a lead | Queries data sources, builds company profile |
| **04 — Qualification** | BANT discovery + lead scoring | Applies consistent qualification logic, ranks leads |
| **05 — Workflow Timeline** | Visual DAG with execution status | Orchestrates parallel/sequential steps |
| **06 — Human Approval** | Approval queue with context | Pauses high-risk actions for review |
| **07 — Outreach + CRM** | Multi-channel outreach + CRM updates | Executes context-aware outreach, keeps records current |
| **08 — Analytics + Cost** | KPIs, cost attribution, ROI | Aggregates performance across all workflows |
| **09 — Audit / Governance** | Complete audit trail | Logs all operations with correlation IDs |

> **[LIVE DEMO URL — Coming after demo validation]**
> **[VIDEO WALKTHROUGH — Coming after demo validation]**

---

## License

Proprietary — All rights reserved.

This repository is provided for investor review purposes only. Unauthorized copying, distribution, or use is prohibited.

---

<div align="center">

**[Request Demo](mailto:demo@growthos.ai)** · **[Architecture](architecture/)** · **[Security](docs/SECURITY.md)**

</div>
