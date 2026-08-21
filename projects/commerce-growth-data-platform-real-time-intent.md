# Making Real-Time Commerce Intent Trustworthy Enough to Activate

I led this 15-terabyte customer-data modernization during my [Rakuten experience from June to December 2023](https://github.com/beastofbayarea/shivam-singh-growth-marketing/blob/main/shivam-singh-growth-marketing.pdf).

Peak customer signals arrived as much as 26 hours late and identities were duplicated across seven systems. Growth teams targeted the same people repeatedly, Sales worked from static lead lists, and the original roadmap prioritized faster ingestion before identity quality.

I reversed that sequence. Faster bad identity would only create more immediate media waste and poorer seller prioritization.

## First, I proved that freshness could change behavior

A two-week regional pilot showed that live intent converted at three times the rate of stale signals. That established the commercial value of lower latency without yet committing the organization to a full rebuild.

I then ran a peak-condition game day. It revealed ghost profiles, overlapping audiences, and conflicting targeting with approximately $2 million in projected media waste. I recommended a three-week launch delay and made golden-record identity resolution the first production requirement.

## The architecture followed the decision sequence

I organized the platform in three layers:

1. Identity integrity: entity resolution, golden records, consent, lineage, and rules for conflicting attributes.
2. Current signals: direct connectors, raw backup, streaming events, and schema contracts.
3. Activation: propensity scores, audience delivery, seller prioritization, and controlled measurement.

The NIST Privacy Framework influenced how I treated data processing, governance, and privacy risk across the lifecycle. METI's AI governance guidance supplied Japan-specific principles for accountable implementation, monitoring, and stakeholder communication.

The architecture therefore did more than move data quickly. It preserved a recoverable raw record, made schema ownership explicit, resolved who a customer was, and carried approved signals into activation.

## Predictive activation kept a protected control

I introduced behavior-based propensity scoring for seller recruitment but retained a random 20% control cohort. That served two purposes. It created a credible estimate of lift, and it prevented the model from permanently excluding unconventional sellers who did not resemble historical winners.

I measured acquisition cost, lead conversion, seller activation, first-year sales, identity quality, audience overlap, and platform reliability together. A predictive score had to improve commercial outcomes without hiding weak segments or amplifying data errors.

## The result across the system

- Peak signal latency fell from 26 hours to under 15 minutes.
- Infrastructure cost declined 30%.
- Customer-acquisition cost fell 20%.
- Lead conversion tripled from 1.8% to 5.4%.
- Recruited-seller first-year sales increased from $12,000 to $28,000.
- The peak event ran without downtime and finished $25 million above the Q4 sales target.

## How I made data quality a growth decision

Engineering, Marketing, Sales, Finance, and Merchant Operations used one scorecard that connected duplicate identity and stale signals to media waste, seller quality, and revenue. That made the launch delay legible as a commercial choice, not technical perfectionism.

My lasting principle is simple: identity first, transport second, prediction third. Real-time activation creates value only when the platform knows whose intent it is observing and can measure what changed because of the action.

## External foundations

These sources supplied the primary privacy and AI-governance methodology. My resume is linked only to establish employment chronology.

| Source | How I applied it |
|---|---|
| [NIST — Privacy Framework 1.0 (2020)](https://www.nist.gov/privacy-framework/privacy-framework) | I used its privacy-risk and data-processing lifecycle to structure identity, consent, lineage, and governance requirements. |
| [METI — Governance Guidelines for Implementation of AI Principles v1.1 (2022)](https://www.meti.go.jp/shingikai/mono_info_service/ai_shakai_jisso/20220128_report.html) | I used its accountable AI implementation and monitoring guidance for predictive activation in Japan. |
