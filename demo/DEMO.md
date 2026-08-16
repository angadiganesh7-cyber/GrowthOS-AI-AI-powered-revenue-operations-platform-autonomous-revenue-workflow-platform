# GrowthOS AI — Demo

> **Status: Coming after demo validation.** Live demo and video walkthrough will be deployed before investor submission.

## Access

> **Live demo URL:** Coming after demo validation
>
> Demo credentials will be provided upon request.

## Investor Walkthrough

This walkthrough shows the complete lead-to-revenue workflow in GrowthOS AI.

---

### 01 — Dashboard

**What you see:** Real-time agent fleet status (10 agents, health, activity), lead pipeline metrics (total, qualified, conversion rate), system health indicators, campaign performance overview.

**What the system is doing:** Aggregating data from all agents, workflows, and CRM into a single operational view. Correlating agent execution status with pipeline outcomes.

**Why it matters:** One screen replaces 6 dashboards across separate tools. You can see the health of the entire revenue operation at a glance.

---

### 02 — Lead Ingestion

**What you see:** Leads entering the system from multiple sources — web forms, CSV uploads, API calls, LinkedIn, email. Each lead is normalized and routed into the workflow engine.

**What the system is doing:** Receiving, validating, de-duplicating, and structuring incoming leads. Assigning source attribution. Triggering the research workflow.

**Why it matters:** No lead falls through the cracks between tools. Every source feeds into one pipeline with one set of rules.

---

### 03 — AI Research

**What you see:** Research agent enriching a lead with company data, tech stack, recent news, intent signals, and organizational context.

**What the system is doing:** Querying public data sources, company databases, and news feeds to build a comprehensive profile. Feeding context to downstream agents.

**Why it matters:** Sales reps start conversations with context, not guesses. Every lead gets the same depth of research, automatically.

---

### 04 — Qualification + Score

**What you see:** Qualification agent running structured discovery (budget, authority, need, timeline). Scoring agent ranking the lead against custom criteria and historical patterns.

**What the system is doing:** Applying consistent qualification logic. Producing a confidence-scored lead rank. Routing qualified leads to the next step; discarding unqualified leads.

**Why it matters:** Consistent, objective qualification across all leads. No more gut-feel scoring. Sales focuses on the highest-value opportunities.

---

### 05 — Workflow Timeline

**What you see:** Visual DAG (directed acyclic graph) with step-by-step execution, timing, and status. Parallel branches, sequential steps, and conditional routing visible in one view.

**What the system is doing:** Orchestrating the workflow through the engine. Managing retries, checkpoints, and dead letter queues. Providing real-time execution updates.

**Why it matters:** Complex processes run deterministically. Every step is auditable. Failures are captured and replayable.

---

### 06 — Human Approval

**What you see:** Approval queue with confidence scores, risk levels, full context, and one-click approve/reject. Review panel showing the lead, research, qualification, and proposed action.

**What the system is doing:** Pausing high-risk or high-value actions. Routing to designated reviewers. Enforcing approval policies before execution.

**Why it matters:** Humans stay in control of critical decisions. Speed of automation with judgment where it matters.

---

### 07 — Outreach + CRM

**What you see:** Multi-channel outreach — email, LinkedIn, WhatsApp, SMS — with context-aware messaging. CRM records updated automatically with activity history.

**What the system is doing:** Executing outreach sequences across channels. Keeping CRM records current without manual data entry. Tracking engagement and responses.

**Why it matters:** Right message, right channel, right timing. No manual data entry. No stale pipeline records.

---

### 08 — Analytics + Cost

**What you see:** Executive KPI dashboard, cost attribution per agent/workflow, ROI metrics, agent leaderboard, performance benchmarks.

**What the system is doing:** Aggregating performance data across all workflows and agents. Calculating cost per lead, cost per qualification, cost per meeting. Attributing outcomes to specific agents and workflow steps.

**Why it matters:** Know exactly what each workflow costs and what it produces. Make data-driven decisions about where to invest.

---

### 09 — Audit / Governance

**What you see:** Complete audit trail of every action, decision, and approval. Timestamped, correlated, and filterable.

**What the system is doing:** Logging all operations with correlation IDs, actor context, and outcome. Providing full traceability for compliance, debugging, and optimization.

**Why it matters:** Full accountability. Know who did what, when, why, and with what outcome.

---

## Architecture Walkthrough

For a detailed architecture walkthrough, see [architecture/ARCHITECTURE.md](../architecture/ARCHITECTURE.md).

## Video Demo

> Video walkthrough coming after demo validation.
>
> **[VIDEO URL — Coming after demo validation]**
