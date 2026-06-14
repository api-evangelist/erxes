# Erxes Rate Limits

Erxes is primarily a self-hosted, open-source platform. Rate limiting behavior depends on the deployment model.

## Self-Hosted (Community & Enterprise Editions)

Rate limits are not imposed by the Erxes software itself; they are governed by the operator's infrastructure configuration. Recommended controls include:

- **API Gateway (Port 4000 — Apollo Router):** Configure rate limiting at the reverse proxy layer (e.g., nginx, Traefik, or Cloudflare) rather than within Erxes.
- **MongoDB:** Connection pool limits apply; default Mongoose pool size is typically 5–10 connections.
- **Redis:** Used for BullMQ job queues; throughput is bounded by Redis instance capacity.
- **Email sending:** Volume constraints depend on the connected SMTP or email provider (e.g., SendGrid, AWS SES).

## Cloud / SaaS Edition

Specific API rate limit values are not publicly documented for the Erxes cloud offering. The following constraints are inferred from plan tiers:

| Plan       | Monthly Email Limit | Contact Limit  |
|------------|--------------------:|---------------:|
| Free       | 5,000               | 5,000          |
| Business   | 5,000               | 25,000         |
| Enterprise | 30,000              | 200,000        |

These are feature/quota limits rather than per-second API rate limits.

## GraphQL API

- The GraphQL Federation API is served through Apollo Router on port 4000 in default self-hosted setups.
- No published per-minute or per-second request rate limits exist in the public documentation.
- For cloud deployments, contact Erxes support to understand any applied throttling policies.

## Recommendations for Integrators

1. Implement exponential back-off when receiving 429 or 503 responses.
2. Cache frequently read data (contacts, pipeline stages) locally to reduce API call volume.
3. Use GraphQL subscriptions for real-time event data rather than polling.
4. For high-volume self-hosted deployments, place a rate-limiting reverse proxy in front of port 4000.

## References

- Erxes Docs: https://erxes.io/docs/introduction
- GitHub Repository: https://github.com/erxes/erxes
