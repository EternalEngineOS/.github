# Repository & Org Settings

These are files, not automation — a maintainer applies them by hand (or via `gh`/API) after
review. Nothing in this repo changes GitHub settings on its own.

## 1. Rename this repository to `.github`

**Do this first.** GitHub only renders an organization's profile README from
`<org>/.github/profile/README.md`. Today the repo is named `EternalEngineOS`, so the org
profile page shows GitHub's placeholder, not our README — renaming to `.github` is what
turns on the profile.

```
gh repo rename .github --repo EternalEngineOS/EternalEngineOS
```

After the rename, verify at `https://github.com/EternalEngineOS` that
`profile/README.md` (this repo) is rendering.

## 2. Repository description

```
The EternalEngine organization profile and community-health files. Product code is private — see eternalengineos.io.
```

## 3. Homepage URL

```
https://eternalengineos.io
```

## 4. Topics

```
saas, small-business, crm, invoicing, scheduling, field-service,
stripe, multi-tenant, ai-agents, service-business, api, mcp
```

## 5. Discussions

**On.** This is the one public, low-stakes surface where prospects, customers, and
integrators can ask questions without opening an issue against a private product repo.
Pin a welcome post pointing to `SUPPORT.md` and the [status page](https://eternalengineos.io/status).

## 6. Org "Verified" badge

**Recommended.** GitHub's blue verified-organization badge (domain verification via a TXT
record on `eternalengineos.io`, under org Settings → Verified domains) is a real,
checkable trust signal — the same category as the website-up badge on the profile page —
and costs nothing but a DNS record. Set it up under the org's own Settings, not this repo.

## 7. Pinned repository

**Pin this repo (`.github`, post-rename)** on the org profile's "Popular repositories"
shelf, if the org has other public repos that would otherwise crowd it out. Since this is
currently the *only* public repo in the org, this is a no-op until a second public repo
exists — but note it now so it isn't missed later.

## 8. Org profile fields (Settings → Profile, organization level)

Confirm these already match the site (no change expected, listed for completeness):

| Field | Value |
|---|---|
| Display name | EternalEngine |
| Description | Home of EternalEngine OS and related services. Solo + AI fleet development. |
| Website | https://eternalengineos.io |
| Email | EE@EternalEngineOS.io |
| Twitter/X | EternalEngineOS |

## 9. Branch protection

Protect `main` on this repo: require a pull request before merging, no force-push, no
deletion. This repo has no CI to require as a check (it's documentation-only).
