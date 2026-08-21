# Sequencing identity, live intent, and seller activation for an AWS customer

Faster data would have amplified the wrong customer.

The commerce client held 15 TB across seven systems. Routine batches took about 12 hours; peak signals arrived as much as 26 hours late. Marketing could advertise products already purchased, sales worked stale seller lists, and one person appeared under multiple POS, commerce, CRM, and web identifiers.

During my AWS role, I led the product/architecture strategy across customer teams, data engineering, marketing, sales, finance, merchant operations, privacy, AWS architects, and executives.

## I reordered the roadmap

The original priority was ingestion speed. I set a different sequence:

1. resolve who the customer or business is and which uses are permitted;
2. move current governed signals against that identity;
3. predict and activate through a measured holdout.

A two-week Vietnam pilot gave one sales cohort live intent and reported 3× conversion versus stale-signal peers. It justified exploration, not an eight-month rebuild: assignment, cohort size, and later-population comparability were not retained.

## The game day produced a reason to delay growth

Peak testing created “ghost profiles.” Faster POS feeds generated identifiers that failed to resolve to existing customers, overlapping segments sent contradictory messages, and CTR fell 15%. The client modeled ~$2 million of media waste.

I recommended a three-week delay. Curated temporary segments kept holiday campaigns running while teams established the match hierarchy, golden-record rule, survivorship, consent/purpose checks, conflict resolution, and stewardship.

That was the critical growth decision: accept a bounded schedule cost to stop real-time infrastructure from multiplying identity error at peak. The $2 million remained a forecast, not a realized saving.

## The platform contract

### Identity

Source identifiers remained intact and linked through deterministic/probabilistic evidence, confidence, lineage, consent, purpose, and a conflict owner. A golden record was reversible; it did not erase source truth.

### Signals

Commerce, POS, CRM, and web events entered through direct connectors/streams with schema contracts. Raw recovery data remained 30 days. Event time and ingestion time were separate. Malformed records entered quarantine. Spend alerts fired at 15% above approved baseline.

### Activation

Every audience or seller queue carried authorization, model/feature version, exclusions, delivery receipt, comparison-group assignment, and outcome feedback.

The [NIST Privacy Framework](https://www.nist.gov/privacy-framework/privacy-framework) informed purpose and governance; Japan’s [METI AI-governance guidance](https://www.meti.go.jp/shingikai/mono_info_service/ai_shakai_jisso/20220128_report.html) supplied an implementation/monitoring benchmark. Neither framework declared the data compliant.

## The workload settled an architecture argument

A stored-procedure identity job and distributed Spark job ran the same test. SQL had not finished after four hours; Spark completed in 45 minutes—at least 195 minutes and 81.25% faster relative to the four-hour mark. Because the SQL run was censored, I do not invent an exact multiple.

The final design paired a recoverable raw layer, streaming event processing, governed analytical storage, and activation outputs. Technology served the contract: no “real time” without replay, identity evidence, schema ownership, permission, and delivery receipts.

## Propensity ranking did not monopolize the market

The seller model used session depth, frequency, search demand, and product interaction. I preserved a random 20% control, both to estimate incrementality and to keep discovering unconventional sellers unlike historical winners.

Measurement continued past a score:

**eligible seller → score/control → sales contact → merchant activation → first transaction → first-year seller GMS**

The model could not claim a merchant who would have joined anyway, and seller GMS was not platform revenue.

## Customer result account

| Outcome | Baseline → target → recorded result | Method |
|---|---|---|
| Peak freshness | 26 h → <15 min → <15 min | Source event to activation-ready signal; >99.04% lower from 1,560 minutes |
| Infrastructure cost | index 100 → reduce → 70 | Comparable workload/capacity and period; 30% lower |
| CAC | index 100 → improve with stable seller mix → 80 | Acquisition spend / activated sellers; 20% lower |
| Seller-lead conversion | 1.8% → improve vs control → 5.4% | Activated sellers / eligible contacted leads; +3.6 points, 3× |
| First-year seller sales/GMS | $12K → grow quality → $28K | Cohort GMS; +$16K, +133.3%, not platform revenue |
| Maintenance | 20 h/week → low-touch → 2 h/week | Logged pipeline maintenance; -18 hours, -90% |
| Peak continuity | baseline absent → no material outage → none recorded | Bounded event observation, not annual availability |

The client finished peak $25 million above its Q4 sales target. Pricing, demand, inventory, marketing, seller mix, and platform all contributed; I present it as business context, not incremental sales caused by my work.

I owned the sequencing decision, architecture, workshops, game-day interpretation, launch-delay recommendation, 20% control, and commercial scorecard. Client leaders owned production data, campaigns, sales action, launch authority, and realized outcomes.

My contribution was to make identity integrity a growth dependency. Once the organization accepted that premise, speed became an advantage instead of a multiplier of duplicate customers and bad decisions.
