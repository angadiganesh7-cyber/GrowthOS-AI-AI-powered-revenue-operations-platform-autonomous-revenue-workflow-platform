# GrowthOS AI — Security Overview

## Security Architecture

GrowthOS AI implements defense-in-depth security across every layer. Security is part of the runtime, not bolted on.

---

## Authentication

- JWT access tokens with short expiry (15 minutes)
- Refresh token rotation with revocation (JTI-based)
- bcrypt password hashing with salt
- OWASP-compliant password complexity requirements
- Account lockout after 5 failed attempts (15-minute cooldown)
- OAuth2 providers (Google, GitHub) with mock implementations for development
- OIDC and SAML 2.0 stubs for enterprise SSO

## Authorization

- Role-Based Access Control (RBAC) with 7 roles:
  - Super Admin, Org Admin, Workspace Admin, Manager, Operator, Viewer, API User
- Granular permissions across 7 domains:
  - System, Organization, Workspace, Agent, Workflow, Billing, Audit
- Resource-level ownership checks
- Attribute-based policy engine

## Multi-Tenancy

- Organization-scoped data isolation
- Context-variable-based tenant context (async-safe)
- Query-level tenant filtering
- Cross-tenant access denial with logging
- Per-tenant quota enforcement

## Tool Authorization

- Central authorization boundary in `ToolExecutor.authorize()`
- Every tool call passes through risk classification
- Blocked tools list for dangerous operations
- Human approval required for high-risk actions
- Token budget enforcement per agent execution

## API Security

- Redis sliding-window rate limiting (configurable per endpoint)
- Stricter limits on authentication endpoints
- Request size limits
- CORS configuration
- OWASP security headers (CSP, HSTS, X-Frame-Options, etc.)

## Data Security

- API keys stored as SHA-256 hashes (never stored raw)
- Webhook payloads verified with HMAC-SHA256 signatures
- Database connections use SSL in production
- Secrets loaded from environment variables (never hardcoded)
- PII filtering on AI outputs

## AI Security

- Input guardrails: prompt injection detection (regex patterns for known attack vectors)
- Output guardrails: PII detection and filtering (credit cards, SSNs, emails, phone numbers)
- Tool risk classification: low/medium/high/critical
- Blocked tools list for dangerous operations
- Human approval required for high-risk actions
- Token budget enforcement per agent execution

## Idempotency

- Key operations (usage recording, cost tracking, CRM updates) are idempotent
- Duplicate execution produces the same result without side effects
- Webhook handling is idempotent — duplicate delivery is safe

## Infrastructure Security

- Docker containers run as non-root user
- Kubernetes deployment with resource limits
- Health probes (liveness, readiness)
- Emergency kill switch for maintenance mode
- Structured logging with correlation IDs
- Prometheus metrics for anomaly detection

## Compliance Readiness

- Complete audit trail of all administrative actions
- Data access logging
- Tenant isolation verification
- Security headers (OWASP recommended)
- Regular dependency scanning (Bandit, Safety)
- Container vulnerability scanning (Trivy)

---

## Security Testing

| Test | Frequency | Tool |
|------|-----------|------|
| Static analysis | Every commit | Bandit |
| Dependency scanning | Nightly | Safety |
| Container scanning | Every build | Trivy |
| Secret scanning | Nightly | Gitleaks |

---

## Reporting Security Issues

To report a security vulnerability, please contact security@growthos.ai.

We take security seriously and will respond to all reports within 24 hours.
