# Erxes GraphQL API

Erxes is an open-source experience operating system (XOS) built on a GraphQL Federation architecture using Apollo Router. The API is organized as a microservices monorepo where each plugin (contacts, inbox, sales, operations, automations, etc.) exposes its own GraphQL subgraph that is federated into a single unified gateway. Core types such as `User`, `Customer`, `Company`, `Tag`, and `Product` are shared across subgraphs via Apollo Federation `@key` directives.

Authentication is JWT-based. Users authenticate via the `login` mutation (email/password) which returns a token, or via Google OAuth / magic-link flows. The token is passed as a Bearer token in the `Authorization` header for subsequent requests. The system also supports OAuth 2.0 client apps with configurable token lifetimes.

**Endpoint:** `http://<host>:4000/graphql` (self-hosted; Apollo Router gateway port 4000 by default)

**Documentation:** https://erxes.io/docs/introduction

**References:**
- Documentation: https://erxes.io/docs/introduction
- GitHub: https://github.com/erxes/erxes
- Core API schemas: https://github.com/erxes/erxes/tree/main/backend/core-api/src/modules
- Sales plugin schemas: https://github.com/erxes/erxes/tree/main/backend/plugins/sales_api/src/modules/sales/graphql/schemas
- Frontline (inbox/ticket) schemas: https://github.com/erxes/erxes/tree/main/backend/plugins/frontline_api/src/modules
- Operation plugin schemas: https://github.com/erxes/erxes/tree/main/backend/plugins/operation_api/src/modules
