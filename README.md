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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

API Evangelist catalog entry for Erxes — the open-source Experience Operating System (XOS) that unifies marketing, sales, operations, and customer support on a single AI-native platform.

## About Erxes

Erxes is a source-available experience management platform built on a GraphQL Federation architecture. It serves as an open-source alternative to HubSpot, Zendesk, Linear, and similar SaaS tools, trusted by over 25,000 organizations. The platform is built with Node.js, TypeScript, MongoDB, Redis, and Apollo Server, exposing a GraphQL API for all core CRM and operational functions.

- **Website:** https://erxes.io
- **Documentation:** https://erxes.io/docs/introduction
- **GitHub Organization:** https://github.com/erxes
- **LinkedIn:** https://www.linkedin.com/company/erxes
- **Pricing:** https://erxes.io/pricing/self-service/frontline

## API

Erxes exposes a GraphQL Federation API through an Apollo Router gateway (port 4000 in self-hosted deployments). The API covers:

- Contacts and companies (CRM)
- Conversations and team inboxes
- Tickets, tasks, and deals
- Sales pipelines
- Marketing automation workflows
- Knowledge base and portals

## Repository Structure

```
erxes/
├── apis.yml                          # APIs.json 0.19 catalog entry
├── plans/
│   └── erxes-plans.md               # Pricing plan details
├── rate-limits/
│   └── erxes-rate-limits.md         # Rate limit documentation
├── finops/
│   └── erxes-finops.md              # Financial operations guidance
└── README.md
```

## Licensing

- **Community Edition:** AGPLv3 (open source, self-hostable)
- **Enterprise Edition:** Proprietary license with additional features and support

## Maintainer

Kin Lane — kin@apievangelist.com
