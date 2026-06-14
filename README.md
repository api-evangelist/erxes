# Erxes

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
