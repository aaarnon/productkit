# 71x Product Metrics Cheat Sheet | Leading Product Metrics Guide

**Author:** Susannah Belcher

**Source:** https://www.hustlebadger.com/metrics/product-metrics/

---

## Overview

Leading product metrics are early indicators by which you can hope to impact lagging outputs like revenue and cohorts. They're easier and quicker to show impact than later stage outputs.

**Types of leading metrics:**
- Traffic and sign-up metrics
- Activation and activity metrics
- Customer surveys

**Warning:** Proving causality between input and output can be tricky—teams often work hard on moving a leading metric only to realize limited output uplift.

---

## Leading vs Lagging Metrics

| Aspect | Leading | Lagging |
|--------|---------|---------|
| **Speed of change** | Fast | Slow |
| **Relation to business** | Predictive | Actual |
| **Team influence** | Large | Small |
| **Examples** | Engagement, adoption, activity | Revenue, profit, ARR, LTV, GMV |

---

## Choosing Good Leading Metrics

### 1. True Driver of Outputs

Moving the input metric should result in positive monetary impact.

**Two ways to discover if input drives output:**
1. **Analysis** — Segmentation or regression to identify tipping points
2. **Trial and error** — Test and learn when data is limited

### 2. Normalized for Periods

Use **Compound Monthly Growth Rate (CMGR)** to understand true underlying growth rate.

- More accurate than mean/average
- Allows benchmarking across initiatives
- Smooths out fluctuations

### 3. Ratio or Rate

Percentage rates are more illustrative of underlying health than absolute numbers.

**Example:** DAU:MAU ratio ensures you're growing long-term active base.

### 4. Commonly Understood

Avoid metrics people don't comprehend. Everyone should agree it's important.

### 5. Influences Behavior

When you look at it, you should be able to make decisions about what to do.

### 6. In Your Remit

The metric should be something your team can move by taking action.

---

## Common Metric Mistakes

| Mistake | Problem |
|---------|---------|
| **Selection bias** | Picking metrics that look good or where you feel affinity |
| **Vanity metrics** | Moving a metric alone has no value |
| **Not benchmarking** | Need to compare against industry, sector, customer benchmarks |

> "Your job is to avoid making decisions off vanity numbers because they are not actionable" — Ben Yoskovitz

---

## Traffic Metrics

### Why Traffic Signals Matter

Traffic data reveals:
1. **Product-market fit** — Low returning users or poor conversion indicate issues
2. **Proposition viability** — Target ICP, pricing, paywall decisions affect traffic
3. **Risk** — High dependency on single traffic source = growth risk
4. **Data maturity** — Poor traffic understanding = poor decision-making

### Paid vs Organic Split

| Characteristic | Paid Traffic | Organic Traffic |
|----------------|--------------|-----------------|
| **Benefits** | Fast, targeted, easy to measure | Slow, follows intent, brand-driven |
| **Weaknesses** | Fleeting, lowest ROI, competitive | Takes effort, technical complexity |
| **Costs** | Ad spend + team | Content + team |

**Key insight:** Paid gets results faster; organic is slower, cheaper, more enduring.

**Organic indicators of product value:**
- **Direct traffic** — Users typing URL directly
- **Brand searches** — Users searching for your brand name
- **Homepage traffic** — Proxy for word of mouth and returning users

### Stickiness: DAU/WAU/MAU

**Definition:** Active users = users with engaged session within time window.

**Stickiness ratios** show if users continue to engage over time:
- DAU:MAU ratio
- Proxy for future cohort metrics

> "WhatsApp's DAU:MAU climbed to 72%. Industry standard is 10-20%, only a handful top 50%" — Sequoia Capital

**Relevance by business type:**
- **Social/games** — Critical (eyeballs for ads)
- **Content sites** — Important (session duration)
- **SaaS** — Less important than MRR
- **E-commerce** — Skip for order metrics

---

## Acquisition Metrics

### Sign-ups / Leads / Downloads

**Warning:** Can easily become untethered from downstream purchase behavior.

**Example problem:**
- Team has goal: increase leads
- Achieves 120% of goal
- But conversion drops from 5% to 2%
- Result: significant revenue drop

**Solution:** Pair with downstream guardrail metric (e.g., conversion rate within 10% of benchmark).

### Conversion Rate

**Formula:** Users who perform action ÷ Total users

**Pitfalls and solutions:**

| Issue | Solution |
|-------|----------|
| Volatility | Normalize: per 100 visitors across 30 days |
| Channel fluctuations | Pick stable subset (organic + direct only) |
| Promotional periods | Be aware of seasonal changes |
| Uncertainty | Use A/B tests |
| No context | Benchmark against industry |

---

## Activation Metrics

### Definitions

| Term | Meaning |
|------|---------|
| **Activated users** | Users who pass the aha moment |
| **Active users** | Users with session in time period (NOT same as activated) |
| **Aha moment** | When user understands product value |
| **Activation rate** | % users hitting activation milestone |

### Value of Activation Metrics

- **Demonstrated value** — Key for EdTech where purchasers want engagement proof
- **Retention impact** — Better activation softens early churn curve

### Common Issues

| Issue | Problem |
|-------|---------|
| **False user definition** | Comparing wrong user sets |
| **False activation definition** | Wrong milestone as aha moment |
| **Vanity** | Conflating download/signup with activation |

### Finding True Activation Point

1. **Track backwards** — From engaged purchasing cohorts to tipping point behaviors
2. **Regression analysis** — Data science identifies actual tipping point

**Requirements for activation rate:**
- Clear, single definition company-wide
- Credible and believable
- Churn reduces after it
- Stick to it consistently

---

## Satisfaction Metrics

### NPS & CSAT

**Limitations:**
- Correlation not causation — Only correlated with high value in some businesses
- Selection bias — Who responds skews numbers
- Can become vanity metrics

**Benefits:**
- Useful with other metrics
- Good practice for engaging users

### Calculating NPS

1. Ask: "How likely (1-10) to recommend to friend?"
2. Bucket responses:
   - 9-10: Promoters
   - 7-8: Passive
   - 1-6: Detractors
3. NPS = % Promoters - % Detractors

**Interpretation:**
- Negative = Bad
- 0-30% = Good
- 30-70% = Great
- 70%+ = Excellent

### Calculating CSAT

- Ask satisfaction on 5 or 10 point scale
- Use weighted average as percentage

**Interpretation:**
- Above 90% = Exceptional
- 86-90% = Great
- 75-85% = Average
- Below 75% = Below average
- Below 60% = Poor

### Operational Satisfaction Metrics

More reliable than surveys:

| Metric | Definition | Use |
|--------|------------|-----|
| **Contact rate** | Contacts ÷ Purchases | Understand user friction |
| **Refund rate** | Refunds ÷ Revenue (or Users) | Identify product issues |

---

## AARRR Framework (Pirate Metrics)

### Customer Journey Stages

| Stage | Focus |
|-------|-------|
| **A**cquisition | Users find your product |
| **A**ctivation | Users engage with your product |
| **R**etention | Users return to your product |
| **R**eferral | Users tell others |
| **R**evenue | Users buy your product |

---

## Key Metrics by Stage

### Acquisition Metrics

| Metric | Definition | Use For |
|--------|------------|---------|
| **User/Session** | Unique visitors / Site visits | Understanding traffic volume |
| **New/Returning** | First-time vs repeat visitors | Growth vs retention balance |
| **Engagement rate** | Sessions >10s or 2+ pageviews | Content/product engagement |
| **Channel/Source/UTM** | Where traffic comes from | Attribution and optimization |
| **Conversion rate** | % progressing through funnel | Measuring friction points |
| **Leads (B2B)** | Form fills requesting contact | Acquisition funnel start |
| **MQL/PQL/SQL** | Qualified leads by source | Lead quality assessment |

### Activation Metrics

| Metric | Definition | Use For |
|--------|------------|---------|
| **Sessions per user** | Average sessions in period | Engagement frequency |
| **DAU/WAU/MAU** | Active users by time period | Product stickiness |
| **Stickiness ratio** | DAU:MAU | Long-term engagement health |
| **Aha moment** | Activation milestone | Critical conversion point |
| **Activation rate** | % passing activation milestone | Funnel efficiency |
| **Time to Value** | Duration to first value | Adoption speed |

### Retention Metrics

| Metric | Definition | Use For |
|--------|------------|---------|
| **CSAT** | Customer satisfaction score | Service quality |
| **NPS** | Net Promoter Score | Product affinity |
| **Refund rate** | % refunded | Product issues |
| **Contact rate** | Support contacts per order | User friction |

### Referral Metrics

| Metric | Definition | Use For |
|--------|------------|---------|
| **Referred users** | Users brought by other users | Referral channel value |
| **Referral rate** | % customers who refer | True promoter count |
| **Virality coefficient** | New users per existing user | Exponential growth potential |

### Revenue Metrics

| Metric | Definition | Use For |
|--------|------------|---------|
| **Conversion to paid** | Trial → Paid % | Propensity to pay |
| **ACV/AOV** | Average contract/order value | Revenue per transaction |
| **MRR/ARR** | Monthly/Annual recurring revenue | Predictable revenue |
| **NRR** | Net revenue retention | True PMF indicator |
| **CLTV** | Customer lifetime value | Acquisition investment |
| **CAC** | Customer acquisition cost | Efficiency measurement |
| **CAC payback** | Time to recoup CAC | Cash flow management |
| **Gross margin** | Revenue - COGS % | Unit economics |

---

## Summary

### Why Bother With Leading Metrics?

1. **Value accelerator** — Finding drivers adds to business playbook
2. **Significant difference** — Right activation point meaningfully changes outcomes
3. **Actionable today** — Move metrics now to impact tomorrow
4. **Knowledge accumulation** — Build experience with what works

### Key Takeaways

1. **Leading metrics predict** — Early indicators of future business performance
2. **Must drive outputs** — Prove causality to revenue/retention
3. **Normalize carefully** — Use CMGR, ratios, consistent time periods
4. **Activation is critical** — But hard to define correctly
5. **Avoid vanity** — Downloads ≠ activation ≠ revenue
6. **Pair with guardrails** — Don't optimize one metric in isolation
7. **Context matters** — Different business types need different metrics
