# Engineering a portable Prime Student campaign under a budget cut

I led a cross-Amazon Prime Student growth program during my AWS tenure. I saw that internal teams were paying to reach the same students and that country-by-country production could not survive a sudden channel restriction. I worked with students, Prime, Video and Music teams, local marketers, creators, media partners, privacy and legal reviewers, analytics, engineering, finance, and Amazon leaders.

## The constraint was a system-design brief

The retained record gives the program a $1 million budget, half the prior year’s spend, and a ten-market remit. Internal audience overlap was 40%; fully bespoke local production was estimated at $2 million; and a later youth-ad policy change throttled 65% of direct-response assets.

I designed three kinds of portability before the policy shock:

- **Audience portability:** participating internal products could suppress an already reached or converted student without distributing direct identifiers broadly.
- **Creative portability:** environment, benefit, hook, format and disclosure were separate approved modules that local teams could recombine.
- **Channel portability:** the proposition could move among paid media, creators, email and owned placements without rebuilding the entire asset.

That turned a budget cut into reusable campaign infrastructure rather than a smaller version of the previous media plan.

## I stopped the internal auction

Prime Student, Video and Music audiences were matched through consented first-party signals. The source describes salted one-way hashes. Hashing an identifier is pseudonymization, not anonymization: a stable token can still link behavior. The design therefore also required approved purpose, limited participants, access control, a privacy assessment, audit records, 30-day retention and deletion.

NIST guidance on [pairwise pseudonymous identifiers](https://pages.nist.gov/800-63-3/sp800-63c.html) is a useful external reference: identifiers should be unguessable, correlation should be justified and bounded to intended parties, and the organization should assess privacy risk. I cite it as a design benchmark, not proof that the campaign implementation conformed to the identity standard.

Audience overlap fell from 40% to 8%, a 32-percentage-point and 80% relative reduction. On a simple $1 million uniform-spend basis, that change implies $320,000 of net duplicate capacity removed, not the source’s $400,000. The $400,000 may describe the original overlap rather than the net improvement; without spend by audience and clearing prices, I do not call it reclaimed savings.

## Creative became a governed component library

I split creative into local environment, member benefit, campaign hook and delivery format. Global teams owned the proposition, brand facts and claim evidence. Local teams chose culturally credible settings, language, offer expression and channel. Japan, for example, required commuter rather than default US dorm imagery.

Approved modules could still produce a bad combination, so every market variant retained offer eligibility, youth-policy review, local claim approval, creator disclosure and a versioned record of what ran. AI-assisted storyboards or copy stayed drafts until a local owner approved them.

Adaptation moved from three days to six hours—66 hours and 91.7% faster. The financial source is internally inconsistent: an 80% reduction from a $2 million baseline implies final cost of $400,000 and $1.6 million saved, while the retained narrative reports $1.2 million saved. Both cannot be true on the same baseline. I report the cycle-time result and preserve the cost conflict for reconciliation.

## The youth-policy blackout tested the design

When platform rules throttled 65% of direct-response assets, engagement fell 30% within 48 hours. I narrowed the team’s work to two decisions: activate compliant creator stories and move eligible remarketing to owned channels. Ten creators received storyboards around how the membership helped during student life, not rigid hard-sell scripts. Replacement content went live within 48 hours.

Creator-led advertising still needed clear commercial disclosure. The FTC’s 2023 guidance on [blurred advertising for children and teens](https://consumer.ftc.gov/consumer-alerts/2023/09/blurred-ads-kids-teens-what-know) recommends a clear separation between ads and content and visible disclosures. It is US guidance; each market still required its own legal and platform review.

I would not claim “100% policy compliance” from the absence of a known violation. The defensible statement is that the replacement assets passed the recorded approval process and no violation is retained in the source.

## Markets had different economic jobs

Drivers were expected to return high average revenue per user, scalers to generate subscriber volume, and incubators to answer localization or channel questions cheaply. The retained allocation was 50% / 30% / 20%.

However, its market table names only eight countries—Japan, the UK, Germany, India, Brazil, Canada, France and Mexico—against a stated ten-market remit. I do not invent the missing two or present the named list as complete.

A small market could retain budget for learning; a large market had to earn marginal spend. I evaluated market and creative cells on incremental subscriber starts, eligible trial-to-paid conversion, retention, contribution margin, and marginal ROAS—not top-line signups alone.

## What the commercial record can and cannot say

| Measure | Baseline or target | Recorded result | Defensible reading |
|---|---:|---:|---|
| Budget | prior-year $2M implied | $1M | 50% reduction if program scopes are equal |
| Audience overlap | 40% | 8% | -32 points, -80% relative; net spend capacity requires auction-level data |
| Adaptation time | 72 h | 6 h | -66 h, -91.7% |
| Creative cost | $2M estimate | 80% lower and $1.2M saved both reported | unresolved arithmetic conflict; do not claim a single saving |
| Direct-response availability | 65% of assets throttled | replacements live in 48 h | operational recovery; final reach and incrementality absent |
| ROAS | 2.5× | 3.6× | +1.1× and +44%; attributed revenue and spend perimeter absent |
| US revenue | $50M target | $48M | 96% of target, $2M short; top-line revenue, not necessarily incremental or campaign-attributed |
| Global subscribers | baseline absent | 3.2M | program-reported volume; paid/organic mix, eligible denominator and incremental holdout absent |

The $48 million US revenue, 3.2 million global subscribers and 3.6× ROAS cannot be put over one $1 million denominator. If all $48 million were campaign-attributed to that spend, gross revenue/spend would be 48×, not 3.6×. They must describe different geographies, attribution scopes, products, or spend pools.

## Provenance and role boundary

The retained project page cites two underlying sources: a Prime Student policy-pivot campaign and a Rakuten Sports ten-market program. It then combines Prime, Amazon internal audiences, Rakuten expansion structure, a current AWS employment period, and one outcome table. That is a composite record.

I have reconstructed the cross-Amazon operating logic and flagged every metric conflict, but the ten-market attribution, subscriber total, and commercial result require the original campaign exports before they should be used as one personal interview claim. The Prime Student program is also a consumer-Amazon product, while this portfolio places it in my AWS tenure. I therefore describe it as a cross-Amazon assignment during that period and do not imply that Prime Student is an AWS product.

I owned the audience and creative system, policy-pivot decision, market portfolio logic, measurement requirements, and execution cadence. Product businesses owned offers and audiences; local teams owned cultural and legal approval; finance owned revenue and spend; privacy owners approved matching. The reusable insight survives the source ambiguity: growth resilience can be designed before the channel fails, but its economics still have to reconcile.
