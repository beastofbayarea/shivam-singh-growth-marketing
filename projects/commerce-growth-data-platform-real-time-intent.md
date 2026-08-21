# Commerce Growth Data Platform - Real-Time Intent and Predictive Activation

## What I worked on

I completed this work during my [Rakuten experience from 2023](https://github.com/beastofbayarea/shivam-singh-growth-marketing/blob/main/shivam-singh-growth-marketing.pdf).

I led a 15 TB customer-data modernization spanning seven systems and turned it into a growth engine for a large commerce business. The program deliberately sequenced identity integrity before real-time pipelines and predictive activation, preventing faster ingestion from amplifying duplicate profiles, wasted media, and poor seller prioritization.

## At a glance

- I reduced peak customer-signal latency from 26 hours to under 15 minutes while lowering infrastructure cost 30%.
- I made golden-record identity resolution the first requirement after stress tests exposed duplicate profiles and roughly $2M in projected media waste.
- I launched behavior-based propensity scoring that reduced CAC 20%, increased lead conversion from 1.8% to 5.4%, and raised recruited-seller first-year sales from $12K to $28K.

## The situation

A large commerce business used stale signals and duplicate customer records during peak events. Growth teams duplicated targeting, sales prioritized static lists, and the original roadmap emphasized ingestion speed before identity quality and measurement trust.

## What I needed to accomplish

I needed to create a resilient growth-data platform that delivered current, trusted intent and measurable activation value across engineering, marketing, sales, finance, and merchant operations.

## What I did

- I used a two-week regional pilot to show that live intent produced three-times-higher conversion before approving the broader rebuild.
- I recommended a three-week launch delay when a game day exposed ghost profiles, overlapping audiences, and conflicting targeting.
- I implemented direct connectors, raw backup, streaming events, schema contracts, entity resolution, and a golden customer record.
- I maintained a random 20% control group around predictive lead scoring to protect unconventional but valuable sellers and separate causal lift from correlation.

## The results

- Signal latency fell below 15 minutes, and infrastructure cost fell 30%.
- CAC declined 20%, and lead conversion tripled to 5.4%.
- Recruited-seller first-year sales increased from $12K to $28K.
- The peak event ran with zero downtime and finished $25M above the Q4 sales target.

## Decisions and trade-offs

- I chose identity integrity over the original launch date.
- I sequenced identity, then pipelines, then predictive activation.
- I used architecture game days and control cohorts to separate causal growth from correlation.

## How I led

I created one commercial and technical scorecard across five functions, translating data quality from an engineering concern into audience trust, merchant growth, and revenue quality.

## Why I chose this approach

I used [NIST - Privacy Framework 1.0 (2020)](https://www.nist.gov/privacy-framework/privacy-framework) to ground privacy-risk, data-processing, and governance framework. I used [METI - Governance Guidelines for Implementation of AI Principles v1.1 (2022)](https://www.meti.go.jp/shingikai/mono_info_service/ai_shakai_jisso/20220128_report.html) to ground japan-specific AI governance foundation.

## Sources and external context

I used independent methodology and market evidence to shape the work. The resume link above is included only to establish the employment timeline.

| Source | How it informed my work | Timing |
|---|---|---|
| [NIST - Privacy Framework 1.0 (2020)](https://www.nist.gov/privacy-framework/privacy-framework) | I used it to ground privacy-risk, data-processing, and governance framework. | — |
| [METI - Governance Guidelines for Implementation of AI Principles v1.1 (2022)](https://www.meti.go.jp/shingikai/mono_info_service/ai_shakai_jisso/20220128_report.html) | I used it to ground japan-specific AI governance foundation. | — |
