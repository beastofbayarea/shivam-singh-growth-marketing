# Letting a retailer earn one camera insight before an enterprise sale

The enterprise trial required twelve weeks of networking, identity, firewall, quota, security, and architecture work led by scarce solution architects. Customers had to commit to a project before learning whether their own footage could improve a store decision.

During my AWS role, I led the product-led growth redesign across store/loss-prevention teams, customer technology/privacy leaders, computer-vision engineering, solution architecture, security, sales, finance, support, and executives.

## One camera. One hour. One viewed insight.

I narrowed the first-value contract to:

- connect one eligible camera;
- process more than one hour of footage; and
- view one traffic, dwell, or interaction insight.

The starter did not promise multi-site production, every camera, live loss-prevention action, or enterprise integration. It promised a bounded proof the retailer could complete under its own authority.

This subtraction changed the acquisition economics. Routine uncertainty moved into product; architects moved downstream to production security, integrations, model fitness, operating procedures, and multi-site expansion.

## The privacy architecture enabled self-service

The original request included live cloud video. I deferred it because continuous upload expanded bandwidth, retention, privacy, and security without improving the first proof.

An in-store edge device processed video and sent lightweight JSON events via MQTT for heatmaps, dwell, traffic, and alerts. Infrastructure-as-code made the deployment reproducible.

Edge processing reduced exposure but did not make event metadata non-sensitive. Purpose, minimization, retention, access, time/location policy, deletion, notice, and model performance across store conditions remained required.

The [NIST Privacy Framework](https://www.nist.gov/privacy-framework/privacy-framework) and [NIST AI RMF](https://doi.org/10.6028/NIST.AI.100-1) informed the governance and measurement perimeter; they were not legal certifications.

## I turned architect memory into a product

Most trial failures came from environment mismatch, not model accuracy. I specified a read-only pre-flight covering service quotas, identity permissions, security groups, network path, and endpoints. It returned the failed condition, why it mattered, and a suggested remediation command.

The diagnostic never executed the change. Customer administrators retained authority. Deployment templates had to pass the same audit in a clean sandbox so a manually repaired snowflake could not be called self-service.

The record’s 15-minute promise and three-week evaluation are two clocks:

- **provisioning:** target 15 minutes after prerequisites pass;
- **evaluation:** camera, approvals, footage, observation, and decision, reduced from 12 weeks to ~3.

## Qualification became evidence of use

A download or demo showed interest. A product-qualified account had completed the proof:

**deploy → connect → process >1 hour → view insight**

Only then did sales and architects assess production value, sites, integrations, risks, and economics. Human expertise moved from setup explanation to expansion of an observed outcome.

I also shifted sales incentive from theoretical signed commitment toward realized paid consumption. Reps benefited when safe use began, cameras/sites expanded, and value persisted. Self-service cannot work economically if compensation still rewards unused capacity.

## Funnel change

| Mechanism | Baseline → target → recorded result | Measurement |
|---|---|---|
| Starter provisioning | architect-scheduled → 15 min after prerequisites → promise retained, observed percentile absent | Template start to healthy first event |
| Full evaluation | 12 weeks → decision quickly → ~3 weeks | Equivalent customer-approval-to-decision boundary; 9 weeks / 75% shorter |
| CAC | index 100 → remove routine specialist labor → 60 | Loaded acquisition cost / acquired customer; 40% lower |
| Paid conversion | index 100 → improve after verified use → 115 | Product-qualified-to-paid or exposed-to-paid denominator must be recovered; +15% source-stated |
| Product qualification | no standard → deploy/process/view → definition established | Final PQA count and PQA-to-paid rate absent |
| Architect capacity | routine trials → complex expansion → redeployed | Hours and opportunity value not retained |

The record supports the operating mechanism and directional funnel changes; it does not support incremental revenue, customer count, vision accuracy, or universal production conversion.

I owned the first-value contract, self-service journey, edge/cloud trade-off, pre-flight, product-qualified definition, specialist handoff, consumption incentive, and funnel account. Engineering owned model/edge/automation; customers controlled cameras and use; privacy/security retained approval; sales owned expansion.

The strategic achievement was a new boundary for enterprise growth: automate repeatable uncertainty, let the customer produce one narrow proof before a large commitment, and reserve experts for the differences where expert judgment creates value.
