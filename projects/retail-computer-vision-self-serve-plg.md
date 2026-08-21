# Letting a retailer earn one camera insight before an enterprise sale

I led product-led growth for a retail computer-vision platform during my AWS role. I saw that retailers had to commit to a long technical project before learning whether their existing camera footage could improve a store decision. I worked with store and loss-prevention teams, customer technology and privacy leaders, product and computer-vision engineers, solutions architects, security, sales, finance, support, and executive sponsors.

## The “premium” trial was twelve weeks of dependency

Each prospect waited for networking, identity, firewall, quota, security and architecture decisions led by a solutions architect. The company spent its most specialized capacity on repeatable setup while the customer had still seen no traffic, dwell or product-interaction insight.

I narrowed the evaluation contract to one camera, more than one hour of eligible footage, and one viewed store insight. The starter path did not promise multi-site production, every camera type, live loss-prevention action or enterprise integration. It promised a bounded proof the retailer could complete under its own control.

I owned the redesign of the entire acquisition motion around that first proof: edge-versus-cloud scope, camera and privacy prerequisites, automated pre-flight, product-qualified usage, specialist escalation, paid-consumption incentives, and funnel measurement. The result compressed an expert-dependent 12-week evaluation to roughly three weeks while reserving architects for multi-site expansion instead of spending scarce field capacity on routine setup.

This was strategic subtraction. Experts remained available after first value for production security, data integration, model fitness, operating procedures and multi-site scale; they were removed from routine trial orchestration.

## The privacy architecture was also the growth architecture

The first design request included live cloud video. I deferred it because continuous upload increased bandwidth, retention, privacy and security scope without improving the first proof.

Video was processed on an edge device in the store. The trial sent lightweight JSON event metadata over MQTT to the cloud for heatmaps, dwell, traffic and alerts. A fixed infrastructure-as-code package made the deployment reproducible.

Edge processing reduced exposure; it did not make the product privacy-free. Event metadata can still describe people or sensitive behavior. The design needed purpose limitation, field minimization, retention, access control, location and time policy, model-performance analysis across conditions, signage or notice as applicable, and a deletion path.

I used the [NIST Privacy Framework](https://www.nist.gov/privacy-framework/privacy-framework) to connect data processing to privacy risk and the [NIST AI Risk Management Framework](https://doi.org/10.6028/NIST.AI.100-1) to structure governance, use mapping, measurement and release decisions. They are voluntary external frameworks, not evidence of legal compliance.

## I moved field knowledge into a pre-flight product

Most failures were environment mismatches rather than vision-model errors. I productized a read-only audit of service quotas, identity permissions, security groups, network path and required endpoints. It returned the failed condition, why it mattered, and a suggested remediation command.

The diagnostic did not execute the change. Customer administrators retained authority and could review the exact action. A deployment template could not be released until it passed the same audit in a clean sandbox, preventing manually repaired “snowflake” trials that customers could not reproduce.

The retained record advertises a 15-minute deployment promise. The end-to-end evaluation still moved to about three weeks. Those are not contradictory if 15 minutes means starter-kit provisioning after prerequisites pass and three weeks includes customer approvals, footage, observation and decision. I keep the two clocks separate.

## Qualification became a product event

A guide download or demo request showed interest. A product-qualified account had done the work:

`deploy starter kit → connect camera → process >1 hour → view insight`

Only then did sales and solution architects enter to determine production value, sites, integrations, risks and commercial scale. That moved human expertise from explaining setup to expanding a demonstrated outcome.

I also changed the sales objective from theoretical contract value at signature toward realized paid consumption. Reps benefited when the retailer started safely, used the product, added cameras or sites, and sustained value. The compensation boundary matters because self-service acquisition fails if sales is still paid to maximize an unused commitment.

## Funnel account

| Measure | Baseline | Product target | Recorded result | Measurement boundary |
|---|---:|---:|---:|---|
| Starter deployment | expert-scheduled | 15 min after prerequisites | source states 15-min promise | provisioning only; no observed percentile or pass rate retained |
| Full evaluation cycle | 12 weeks | reduce time to a decision | ~3 weeks | 9 weeks and 75% shorter; start/end events must include equivalent customer approvals |
| Customer-acquisition cost | index 100 | remove routine specialist work | index 60 | 40% lower; acquisition definition, loaded labor and cohort absent |
| Paid conversion | baseline index 100 | improve after verified use | index 115 | source states +15%; relative versus points and denominator absent |
| Product-qualified usage | no standard | deployed + processed + viewed | definition established | final count and PQA-to-paid rate absent |
| Specialist capacity | routine mid-market trials | complex expansion | redeployed | hours and opportunity value not retained |

The record supports an operating mechanism—setup knowledge absorbed into the product—and three directional funnel results. It does not support incremental revenue, number of customers, model accuracy, or a claim that every trial became production.

## My growth ownership

I owned the first-value contract, default self-service journey, edge-versus-cloud product trade-off, pre-flight requirements, product-qualified account definition, specialist handoff, consumption incentive, and funnel measurement. Engineering owned the model, edge runtime and automation. Customer owners controlled cameras and operating use. Privacy and security specialists retained approval. Sales owned expansion.

The strategic outcome was a new economic boundary for an enterprise product: automate the repeatable uncertainty, let customers see a narrow result before a large commitment, and reserve experts for differences that genuinely require judgement.
