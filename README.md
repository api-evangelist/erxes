# Erxes

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Open-source Experience Operating System (XOS) that unifies marketing, sales, operations and support in one self-hostable platform, positioned as a replacement for HubSpot, Zendesk, Linear and Wix. The machine surface is a GraphQL Federation API served by an Apollo Router gateway — there is no REST API and no OpenAPI — covering contacts, companies, products, tags, documents, brands, organization structure, team members and automations in the core subgraph, plus sales, frontline (inbox/tickets), operation (projects/tasks/cycles) and block plugin subgraphs. Authentication is OAuth 2.0 Device Authorization Grant with per-tenant clients and a documented 34-scope vocabulary. erxes ships the Community Edition under AGPL-3.0 alongside a proprietary Enterprise Edition, publishes its own agent plugin and agent skills, and releases roughly once per merge day.

**Areas:** GraphQL · CRM · Customer Experience · Open Source · Marketing Automation · Sales Pipeline · Help Desk · Ticketing · Team Inbox · Self-Hosted · Apollo Federation · Project Management

## Erxes on APIs.io

Everything profiled for Erxes is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/erxes/](https://apis.io/providers/erxes/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [Erxes GraphQL API](https://apis.io/apis/erxes/graphql-api/) — GraphQL Federation API powering the erxes XOS platform. An Apollo Router gateway federates one subgraph per plugin — core (contacts, companies, products,…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Erxes Webhooks](https://apis.io/asyncapis/erxes/erxes-webhooks/)

#### GraphQL (1)

GraphQL schemas.

- [Erxes GraphQL API](https://apis.io/graphqls/erxes/erxes-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [erxes](https://apis.io/servers/erxes/erxes/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Erxes Authentication](https://apis.io/security/erxes/erxes-authentication/)
- [Erxes Domain Security](https://apis.io/security/erxes/erxes-domain-security/)
- [Erxes Vulnerability Disclosure](https://apis.io/security/erxes/erxes-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Erxes Scopes](https://apis.io/scopes/erxes/erxes-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Erxes Plans Pricing](https://apis.io/plans/erxes/erxes-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Erxes Rate Limits](https://apis.io/rate-limits/erxes/erxes-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://erxes.io)
- [Documentation](https://erxes.io/docs/introduction)
- [Getting started](https://docs.erxes.io/self-hosting)
- [API reference](https://github.com/erxes/erxes-skills/blob/main/agent-plugin/erxes-next/erxes-graphql-api.md)
- [Pricing](https://erxes.io/pricing/self-service/frontline)
- [Sign up](https://erxes.io/auth/signup)
- [Support](https://erxes.io/discussions)
- [Blog](https://erxes.io/blogs)
- [Security](https://github.com/erxes/erxes/blob/main/SECURITY.md)
- [Terms of service](https://erxes.io/legal/terms)
- [Privacy policy](https://erxes.io/legal/privacy)
- [GitHub](https://github.com/erxes)
- [Status](https://status.erxes.io)

## API Evangelist rating

**Kin Score 65.7** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 80.4 |
| Contract quality | 46.9 |
| Contract governance | 4.5 |
| Operational transparency | 81.6 |
| Developer ergonomics | 78.6 |
| Access clarity | 76.3 |

**Agent readiness 28.8** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 40.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/erxes/](https://apis.io/providers/erxes/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Erxes: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/erxes/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
