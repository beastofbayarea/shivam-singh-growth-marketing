# Sequencing identity, live intent, and seller activation for an AWS customer

I led product and architecture strategy for a commerce customer-data program during my AWS role. I saw that marketers and sales teams were acting on stale behavior and duplicate customer identities. I worked with the customer’s shoppers and prospective sellers, data engineering, marketing, sales, finance, merchant operations, privacy teams, AWS architects, and executive owners.

## Speed would have amplified the wrong customer

The customer held 15 terabytes across seven systems. Normal batches took about 12 hours and peak signals arrived as much as 26 hours late. Marketing could target products a shopper had already bought; sales worked from static seller lists; and one person could appear under several point-of-sale, commerce, CRM, or web identifiers.

The initial roadmap prioritized faster ingestion. I changed the product sequence to:

1. define who the person or business is and which uses are permitted;
2. move current, governed signals against that identity; then
3. predict and activate only with a protected comparison group.

A two-week Vietnam pilot gave one sales cohort live intent alerts and reported three times the conversion of stale-signal peers. It justified deeper investigation, not the entire eight-month rebuild: the source does not retain cohort size, assignment, or whether the pilot population matched the later rollout.

## A game day changed the launch decision

Peak testing exposed “ghost profiles.” Faster point-of-sale ingestion created new identifiers that did not resolve to existing customers, and overlapping segments sent contradictory ads. CTR declined 15% during the test, and the customer projected roughly $2 million of media waste.

I recommended delaying launch by three weeks. Temporary, manually curated segments kept holiday campaigns operating while data owners established the golden-record rule, match hierarchy, survivorship logic, consent and purpose checks, conflict resolution, and stewardship.

I delayed the launch to protect growth from bad identity at peak season, then set the architecture and operating sequence that earned it back. The program joined a 26-hour freshness problem, customer resolution, streaming and replay, privacy purpose, model treatment, seller activation, sales action, and Finance's commercial account—so a three-week delay could unlock sub-15-minute intent and a threefold seller-lead conversion result without multiplying duplicate customers.

The $2 million was a customer forecast of avoidable spend, not a realized loss or saving. The decision to delay belonged to the customer; I owned the diagnosis, architectural recommendation, sequencing, and executive evidence.

## The platform contract

**Identity layer.** Source identifiers, deterministic and probabilistic match evidence, consent state, purpose, lineage, confidence, and an owner for conflict. A golden record did not erase source records; it linked them with a reversible decision.

**Signal layer.** Direct connectors and streams from commerce, point of sale, CRM and web; schema contracts; raw recovery data retained for 30 days; event-time and ingestion-time monitoring; quarantine for malformed records; and a spend alert at 15% above the approved baseline.

**Activation layer.** Authorized audiences, ranked seller queues, model and feature versions, exclusion rules, delivery receipts, holdouts, and outcome feedback.

The [NIST Privacy Framework](https://www.nist.gov/privacy-framework/privacy-framework) informed the privacy-risk lifecycle around data mapping, purpose, consent, governance, and control. Japan’s [METI AI-governance guidance](https://www.meti.go.jp/shingikai/mono_info_service/ai_shakai_jisso/20220128_report.html) provided a contemporaneous external benchmark for accountable implementation and monitoring. Neither framework makes a dataset compliant by itself.

## I used the workload to settle an architecture argument

A legacy stored-procedure path and a distributed Spark identity-resolution job ran against the same test. The SQL job had not finished after four hours; the distributed job completed in 45 minutes—at least 195 minutes and 81.25% faster relative to the four-hour mark. Because the first job was censored at four hours, I do not claim an exact speed multiple.

The resulting design used a recoverable raw layer, streaming event processing, a governed analytical store, and activation outputs. Technology was subordinate to the contract: freshness without replay, schema ownership, identity evidence, and downstream receipts would not be trustworthy real time.

## Propensity did not get every lead

The seller model used session depth, frequency, search demand, and product interaction to rank likely, valuable sellers. I retained a random 20% control. That produced an estimate of incremental conversion and continued to expose the team to unconventional sellers unlike historical winners.

The measurement chain ran from eligible seller to score, sales contact, merchant activation, first transaction, and first-year gross merchandise sales. Model ranking could not claim value for a seller who would have joined anyway, and seller GMS was not Rakuten or customer revenue.

## What the customer recorded

| System or growth measure | Baseline | Recorded result | Calculation and boundary |
|---|---:|---:|---|
| Peak signal latency | 26 h | <15 min | from 1,560 to <15 minutes; >99.04% reduction in worst-case source-to-activation freshness |
| Infrastructure cost | index 100 | index 70 | 30% lower; workload, reserved capacity, and period not retained |
| Customer-acquisition cost | index 100 | index 80 | 20% lower; must be read with seller mix and control outcomes |
| Seller-lead conversion | 1.8% | 5.4% | +3.6 points, +200% relative, exactly 3× |
| First-year seller sales/GMS | $12K | $28K | +$16K and +133.3%; source uses both “sales” and “GMS,” so it is not presented as platform revenue |
| Pipeline maintenance | 20 h/week | 2 h/week | 18 hours and 90% lower |
| Peak-event availability | not retained | no downtime recorded | bounded to the observed event, not annual availability |

The customer also finished the peak period $25 million above its Q4 sales target. That is an actual-versus-plan variance across pricing, demand, inventory, marketing, seller mix, and platform performance. I report it as customer business context, not incremental sales caused by the data platform or my work.

## Attribution correction

An earlier portfolio version placed this project under my Rakuten internship. The retained source repeatedly and explicitly describes it as an AWS customer engagement and distinguishes my AWS product/architecture role from the customer’s operating and investment authority. I have corrected the career assignment here and in the portfolio guide.

I owned the decision sequence, target architecture, customer workshops, game-day evidence, launch recommendation, model-control requirement, and shared commercial scorecard. Customer leaders owned production data, campaigns, sales action, launch approval, and realized results. That boundary makes the story stronger: my contribution was turning identity integrity from “data cleanup” into the prerequisite for reliable growth.
