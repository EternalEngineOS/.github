# Security Policy

EternalEngine welcomes coordinated disclosure from security researchers.

## Reporting a vulnerability

Email **EE@eternalengineos.io** with the subject line `Security report` and your reproduction
steps. We acknowledge every report within two business days. Good-faith research reported
through this channel will never be met with legal action.

Do not open a public GitHub issue for a suspected vulnerability — issues in this repository
are public by default and issues are not the right channel for anything that could put
customer data at risk.

## What to include

- The affected URL, endpoint, or app.
- Steps to reproduce, or a proof-of-concept.
- The impact as you understand it.

## Response targets

When a report is confirmed, these are the internal remediation targets our engineering
process is built around:

| Severity | Remediation target |
|---|---|
| Critical | 24 hours |
| High | 72 hours |
| Medium | 7 days |
| Low | 30 days |

## Scope

In scope: `eternalengineos.io`, `app.eternalengineos.io`, `scrollforge.io`, the public API and
the MCP server described on the [developers page](https://eternalengineos.io/developers).
Out of scope: denial of service, social engineering of staff or customers, and findings on
third-party services we do not operate (payment processing is handled by Stripe).

## More detail

Full description of our security architecture — encryption, tenant isolation, access
controls, secure development, and our compliance posture — is in
[`docs/security-and-compliance.md`](docs/security-and-compliance.md) and on the
[public security page](https://eternalengineos.io/security).
