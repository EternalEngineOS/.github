# Security & Compliance

Mirrored from the [security page](https://eternalengineos.io/security) — that page is the
source of truth; this document exists so the same facts are discoverable from GitHub.

## Data encryption

- TLS 1.3 protects every connection in transit.
- Backups and cold-storage archives are encrypted (X25519/age, restic).
- Secrets live in an encrypted vault — never in code or config.

## Tenant isolation

Every organization operates in a completely isolated environment with row-level security
(RLS) enforced at the database level. No cross-tenant data access is possible.

## Access controls

- Role-based access control (RBAC) with granular permissions.
- JWT authentication tokens.
- Complete audit trails for every action.

## Secure infrastructure

- Containerized services with network segmentation and an edge WAF (Cloudflare).
- Automated daily backups with point-in-time recovery.

## Secure development

- Static analysis (CodeQL + Semgrep) on every change.
- Dependency review, vulnerability audit, and secret scanning.
- Signed commits and a protected release branch.

## Trust nothing by default

- Schema validation on all external inputs.
- Parameterized SQL only — no string interpolation.
- Deny-by-default authentication on every endpoint.

## Engineering governance

Every change ships through an automated gate in the build pipeline that enforces these
rules — tenant isolation from the auth context only, parameterized queries, validated
inputs, no secrets in code or logs, structured audit logging — rather than relying on good
intentions. Aligned to OWASP ASVS and NIST SP 800-218 (SSDF); software bills of materials
and build provenance are produced for every release.

## Compliance posture (honesty over badges)

We engineer against OWASP ASVS and NIST SP 800-218 today. GDPR compliance is in progress.
SOC 2 Type II and ISO 27001 are on the roadmap — not yet certified. We will not display a
certification we haven't earned.

## Vulnerability response targets

| Severity | Remediation target |
|---|---|
| Critical | 24 hours |
| High | 72 hours |
| Medium | 7 days |
| Low | 30 days |

Report a vulnerability: see [`../SECURITY.md`](../SECURITY.md).

## Your data and requests

These rights are honored for every user, in every jurisdiction:

| Request | How | Response time |
|---|---|---|
| Copy of your data (access) | Email, or in-app CSV export | Within 30 days |
| Export / portability | In-app CSV export; assisted bulk export on request | Self-serve / within 30 days |
| Correction | Edit in-app, or email | Self-serve / within 30 days |
| Deletion | Settings → Danger Zone → Delete Account, or email | Immediate deactivation; permanent deletion from production within 90 days |
| Marketing opt-out | Unsubscribe link, or email | Immediate |
| Withdraw consent | In-app notice settings, or email | Immediate in-app / within 30 days by email |

Full detail: [Your Data & Requests](https://eternalengineos.io/data-requests).

## Governing documents

- [Data Processing Agreement](https://eternalengineos.io/dpa) — you are the controller of
  your customers' data; we are the processor, acting only on your documented instructions.
- [Privacy Policy](https://eternalengineos.io/privacy)
- [Terms of Service](https://eternalengineos.io/terms)
