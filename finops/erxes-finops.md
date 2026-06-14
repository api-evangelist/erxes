# Erxes FinOps

Financial operations guidance for teams evaluating or running Erxes as part of their technology stack.

## Deployment Cost Models

### Self-Hosted (Open Source)

The Erxes Community Edition (AGPLv3) is free to use but carries infrastructure costs:

| Component         | Minimum Spec                    | Estimated Monthly Cost (Cloud VM) |
|-------------------|---------------------------------|-----------------------------------|
| Application server| 4 vCPU, 8 GB RAM               | $30–$80 (AWS t3.xlarge or equiv.) |
| MongoDB           | 4 GB RAM, 50 GB SSD             | $40–$100 (Atlas M10 or self-managed) |
| Redis             | 1 GB RAM                        | $15–$30 (managed or self-managed) |
| Elasticsearch     | 4 GB RAM (optional, for search) | $40–$80 (managed)                 |
| Object storage    | Varies (file attachments)       | $5–$20 (S3 or compatible)         |
| **Total estimate**|                                 | **$130–$310/month**               |

Self-hosted total cost of ownership (TCO) also includes engineering time for setup, maintenance, upgrades, and security patching.

### Cloud / SaaS Edition

Erxes offers managed cloud hosting with per-module pricing. For the Frontline module:

| Plan       | Cost         | Contact Limit | Team Members |
|------------|--------------|---------------|--------------|
| Free       | $0/month     | 5,000         | 1            |
| Business   | Contact sales| 25,000        | 5            |
| Enterprise | Contact sales| 200,000       | 10           |

- Business and Enterprise pricing is not publicly listed; requires contacting Erxes sales.
- Third-party estimates (Capterra, TrustRadius) suggest plans ranging from $0–$20/seat.
- Add-ons (Premium Support, Custom Onboarding, Migration) carry additional costs not publicly stated.

## Cost Optimization Strategies

### Self-Hosted

1. **Right-size MongoDB early.** A single Atlas M10 cluster ($57/month) handles most small-to-mid deployments. Avoid over-provisioning.
2. **Disable Elasticsearch** if full-text search is not required; it is optional and resource-intensive.
3. **Use spot/preemptible instances** for non-production environments to cut VM costs by 60–80%.
4. **Consolidate Redis** with other services sharing a Redis instance where workloads permit.
5. **Enable Redis persistence** only if BullMQ job durability is required — AOF logging increases I/O costs.

### Cloud SaaS

1. **Start on Free tier** to validate the platform before committing to paid plans.
2. **Audit contact list hygiene** — contact limits are the primary constraint on plan tier, so deduplication and suppression reduce costs.
3. **Negotiate annual contracts** for Business and Enterprise tiers, which typically yield 15–25% discounts vs. month-to-month.

## Budget Planning

- **Pilot / POC:** $0 (Free cloud tier or self-hosted on a single $40/month VM)
- **Small team (5–10 users):** $50–$200/month self-hosted or Business cloud tier
- **Mid-market (50+ users):** Enterprise tier or self-hosted on dedicated infrastructure ($300–$600/month infra)
- **Large enterprise:** Custom pricing; self-hosted with dedicated DBAs and DevOps overhead

## Licensing Considerations

- **AGPLv3 (Community):** Free to use and modify; requires publishing modifications if you distribute the software.
- **Enterprise License:** Proprietary; unlocks additional modules and support. Contact Erxes for pricing.
- No per-API-call charges in either model.

## References

- Pricing: https://erxes.io/pricing/self-service/frontline
- GitHub: https://github.com/erxes/erxes
- Capterra: https://www.capterra.com/p/194629/erxes/
- TrustRadius: https://www.trustradius.com/products/erxes/pricing
