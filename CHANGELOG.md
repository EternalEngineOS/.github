# Changelog

Public release notes for the EternalEngine platform, mirrored from the
[changelog on eternalengineos.io](https://eternalengineos.io/changelog). Newest first.

## v1.2.0 — Seventeen Apps Installable (2026-06-15)

Seven apps graduated from the coming-soon catalog to installable, taking the launch catalog
from ten apps to seventeen:

- **NeuralGrid** — AI office manager: summaries, drafts, and answers across your data.
- **WikiShelf** — the built-in EternalEngine guide and your own team wiki.
- **NotifyStack** — transactional email and notification delivery.
- **CrewGrid** — crew scheduling and dispatch.
- **StockShelf** — inventory and materials tracking.
- **SignSeal** — e-signature for estimates, contracts, and change orders.
- **FlowRelay** — workflow automation between apps.

The coming-soon catalog stood at 23 apps after this release, matching the pricing page and
the in-app store at the time.

## v1.1.0 — June Update: New Site, Sharper Legal, Honest Status (2026-06-11)

A full refresh across everything public-facing:

- **New website** — redesigned end to end, with a new type system and motion design that
  respects reduced-motion preferences.
- **Terms of Service** — rewritten and grounded in the product as it existed then: early-access
  status, provisional pricing disclosure, plans and cancellation, add-on services, PayGate /
  Stripe Connect terms, PostFrame email sending rules, and AI usage.
- **Privacy Policy** — updated with our actual service providers (Stripe, Cloudflare, AI
  model providers), an AI-and-your-data section, and a 30-day commitment to answer privacy
  rights requests for every user, in every jurisdiction.
- **Security page** — expanded with the secure-development pipeline (CodeQL + Semgrep on
  every change, dependency review, secret scanning, signed commits), vulnerability
  remediation targets (Critical: 24h, High: 72h), and a coordinated-disclosure channel for
  researchers.

## v1.0.0 — Platform Launch (2026-02-22)

EternalEngine went live. Ten apps installable on day one:

- **ScrollForge** — the in-app store and launcher.
- **ClientForge** — CRM with contacts, accounts, deals, leads, pipelines, custom fields,
  workflows, and email sequences.
- **ThreadRealm** — cross-customer community forum with boards, threads, comments, votes,
  polls, reactions, DMs, events, and moderation.
- **PostFrame** — transactional and marketing email with SPF/DKIM/DMARC, open and click
  tracking, templates, and webhooks.
- **PayGate** — in-app payment processing, with a Free tier (2.9% + $0.30, up to $10K/mo)
  included on every plan.
- **BookSlot** — appointment scheduling with Google and Outlook sync, a customer-facing
  booking page, and recurring appointments.
- **BidForge** — line-item estimates, takeoffs with CSV export, reusable templates, digital
  signing, and auto-flow to TitanLedger.
- **ProjectPath** — projects, tasks with checklists, daily logs, inspections, time tracking,
  and milestone-triggered invoices.
- **AssetVault** — cloud file storage with folders, version history, tagging, multipart
  uploads, and tenant isolation.
- **TitanLedger** — PDF invoices, full lifecycle (issue/send/approve/bill/refund/void), aging
  reports, and multi-currency books.

Launch-day pricing (Starter $39, Pro $89, Business $149) was superseded on 2026-08-28 by the
current six-tier ladder — see [`docs/pricing.md`](docs/pricing.md) for what is sold today.

---

*This file mirrors the product changelog for GitHub visibility. The
[live changelog](https://eternalengineos.io/changelog) is the source of truth.*
