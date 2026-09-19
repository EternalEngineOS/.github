# Security Policy

EternalEngine welcomes coordinated disclosure from security researchers.

## Reporting a vulnerability

Email **security@eternalengineos.io** with reproduction steps. Good-faith research reported
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

## Known documentation drift

Our published `security.txt` (RFC 9116, at `/.well-known/security.txt` on the marketing
site) currently lists `security@eternalengine.io` and `www.eternalengine.io` — the wrong
domain (missing the `os`). The correct, monitored addresses are **security@eternalengineos.io**
(this file) and **info@eternalengineos.io** (the contact published on the site's
[security page](https://eternalengineos.io/security)). This is noted here so a researcher
who finds the stale file is not misdirected; the site file is being corrected separately.

## More detail

Full description of our security architecture — encryption, tenant isolation, access
controls, secure development, and our compliance posture — is in
[`docs/security-and-compliance.md`](docs/security-and-compliance.md) and on the
[public security page](https://eternalengineos.io/security).
