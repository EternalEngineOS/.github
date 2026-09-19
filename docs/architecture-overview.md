# Architecture Overview (public level)

This is what we say publicly about how EternalEngine is built. It intentionally stops at
the level a customer or integrator needs — no internal service names, hostnames, or
infrastructure details beyond what we already publish on the
[security page](https://eternalengineos.io/security).

## Multi-tenant SaaS, one account for every app

EternalEngine is a single multi-tenant platform: one account, one login, and one bill cover
every app in the catalog. There is no per-app sign-up and no separate subscription to
provision — the apps available to you are determined by your plan
(see [`docs/pricing.md`](pricing.md)).

## Tenant isolation

Every organization operates in a completely isolated environment. Row-level security is
enforced at the database level, so no cross-tenant data access is possible — this is a
database-layer guarantee, not an application-layer convention.

## Payments

Billing and payment processing run on Stripe. PayGate, our native checkout and payments
app, gives customers one all-in processing rate with no separate processor fee — see the
[PayGate feature page](https://eternalengineos.io/features/paygate/).

## Edge and infrastructure

- **Edge / WAF** — network segmentation and edge protection via Cloudflare.
- **Encryption in transit** — TLS 1.3 on every connection.
- **Encryption at rest** — backups and cold-storage archives are encrypted.
- **Containerized services** with automated daily backups and point-in-time recovery.

Full detail: [`docs/security-and-compliance.md`](security-and-compliance.md) and the
[security page](https://eternalengineos.io/security).

## API and AI agent access

A read-only public API and an MCP (Model Context Protocol) server let developers and AI
agents read data with their own API key, from their own machine — no write endpoints exist
in the public spec. See the [Developers page](https://eternalengineos.io/developers).

## What is not public

The application source code, internal service topology, and deployment tooling are private.
This document describes the externally observable architecture only — the facts a customer
or integrator needs, each of which is already stated on a public page linked above.
