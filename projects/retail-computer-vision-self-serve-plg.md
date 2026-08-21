# Letting Retailers Prove Computer-Vision Value Before a Sales Cycle

I led this product-led growth work during my [AWS experience beginning in July 2024](https://github.com/beastofbayarea/shivam-singh-growth-marketing/blob/main/shivam-singh-growth-marketing.pdf).

Retailers wanted insights from their existing cameras, but evaluating the product required about 12 weeks of custom networking, identity, security, and solutions-architect work. The company was spending expert time before the customer had seen one useful result.

I replaced that white-glove entry point with a self-service path designed around one promise: connect one camera and reach one retail insight safely.

## I narrowed the first-value unit

The initial trial did not attempt every enterprise integration. It used a starter kit and a fixed infrastructure-as-code deployment that could process one camera, produce lightweight metadata, and display one insight.

Video stayed at the edge. Only the information needed for the insight moved to the cloud. NIST's Privacy Framework influenced this data-minimization choice, while the AI Risk Management Framework shaped how I mapped the use, measured performance and harm, assigned ownership, and managed release risk.

I deferred live video streaming because it increased privacy, bandwidth, and security complexity without improving the first proof of value.

## Pre-flight diagnostics replaced avoidable calls

Most trial failures came from predictable environment conditions: quotas, security groups, IAM, and network paths. I built a read-only pre-flight audit that checked those conditions before deployment and returned specific remediation guidance.

The diagnostic did not silently modify the customer's environment. It made the problem visible and let the customer or administrator choose the correction. This removed routine back-and-forth while preserving enterprise control.

## Qualification moved into the product

A content download or demo request was a weak signal of buying intent. I defined a product-qualified account as one that had deployed the kit, processed footage, and viewed an insight.

Sales and solutions architects entered after that event to help with multi-site rollout, production security, data integration, and enterprise operating design. I also aligned sales rewards with realized consumption rather than theoretical contract size, so the commercial motion reinforced durable use.

## What changed

- The evaluation cycle fell roughly 75%, from 12 weeks to about three.
- Customer-acquisition cost declined 40%.
- Paid conversion increased 15%.
- Specialist capacity moved from repeatable trial setup to higher-value enterprise expansion.

## Why the result was a product change, not a funnel trick

Self-service worked because the product absorbed setup knowledge that previously lived in meetings. The fixed first-value unit, edge-processing boundary, infrastructure automation, and pre-flight audit made the evaluation reproducible.

That is the product-led growth standard I use for complex enterprise technology: let the product demonstrate a meaningful outcome on a safe, narrow path; bring experts in when the customer's context truly requires expertise.

## External foundations

These sources supplied the primary AI-governance and privacy methodology. My resume is linked only for employment chronology.

| Source | How I applied it |
|---|---|
| [NIST — AI Risk Management Framework 1.0 (2023)](https://doi.org/10.6028/NIST.AI.100-1) | I used its govern-map-measure-manage cycle to structure the bounded computer-vision trial and release gates. |
| [NIST — Privacy Framework 1.0 (2020)](https://www.nist.gov/privacy-framework/privacy-framework) | I used its data-processing and privacy-risk principles to keep video at the edge and minimize cloud data. |
