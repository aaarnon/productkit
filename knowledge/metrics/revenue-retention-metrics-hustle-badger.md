# Revenue and Retention Metrics Guide

**Author:** Susannah Belcher (Hustle Badger co-founder, ex Rocket Internet, Groupon, DataCamp)

**Source:** https://www.hustlebadger.com/metrics/product-success-metrics/

---

## Overview

Revenue, profit, and retention are **lagging metrics**—a scorecard of how you did in the past that defines current success and potential future investments.

**Why these matter:**
1. **They're the metrics which matter** — Retained customers, generated revenue, and profit drive the business
2. **They are your problem** — Product's performance is the core driver
3. **Commonly misunderstood** — People define and calculate them differently

---

## Best Practices

- **Agree on understood definition** — Wrong definition can be fatal to credibility
- **Make definition transparent** — Add footnotes or definition tables
- **Don't massage the metric** — Goal is true health, not pretty pictures

> "You can't simply apply or copy the churn reporting technique from one business to another" — Olga Berezovsky

---

## Retention Metrics

### Cohorts

Cohorted views show retention by time period for different user behaviors.

#### Common Cohort Views

| Type | What It Tracks |
|------|----------------|
| **Traffic** | Repeat visits within time period |
| **Engagement** | Core actions performed within time period |
| **Purchase** | Purchases performed within time period |
| **User** | Users still paying within time period |
| **Revenue** | Revenue retained within time period |

#### How to Build Cohort Tables

1. All defined users
2. In a defined time period (pick starting date)
3. Who perform X action in next period (same length)
4. Repeat for total number of time periods

#### What Cohorts Tell You

- **Understand users** — Which cohorts are stickier or churn more
- **Track performance** — Basis for Finance's quarterly planning
- **Find problems** — Quickly show if business is viable
- **Make interventions** — Win customers back or foster engagement

#### Common Cohort Mistakes

- **Vanity metrics** — Use hard output metrics (purchase count, retained revenue)
- **Wrong time periods** — Social apps: hourly/daily. Subscriptions: monthly. E-commerce: 28-day
- **Not segmenting** — Segment by customer profile, geography, channel, device

> "Sometimes the cohorts are the cohorts are the cohorts" — Oli Samwer, Rocket Internet

---

### Churn

Churn is the opposite of retention, expressed as percentage.

#### Types of Churn

| Type | Definition | Useful For |
|------|------------|------------|
| **Gross churn** | Revenue/users lost ÷ starting revenue/users | Understanding replacement needs |
| **Net churn** | (Lost - Gained) ÷ starting | Understanding if business growing/shrinking |

#### Key Churn Metrics for PMs

- **Gross user churn** — How many users quit your product (especially important in Enterprise where big contracts skew revenue)
- **Voluntary vs Involuntary** — Involuntary = card expired (fix via payment optimization). Voluntary = user cancels (needs deeper intervention)

---

## Monetary Metrics

### Income Metrics Overview

| Metric | Definition | When Recognized |
|--------|------------|-----------------|
| **Revenue** | Money recognized when delivering service | As service delivered |
| **Bookings** | Contracted future revenue | When contract signed |
| **Cash** | Money hitting bank account | When payment received |

#### Example: $12,000 Annual Subscription

- **Dec 1** — Contract signed → Bookings
- **Jan 1** — Subscription activated → $1,000/month Revenue (1/12th)
- **Mar 30** — Full payment received → $12,000 Cash

---

### ARR / MRR (Recurring Revenue)

Only for subscription/SaaS businesses.

**Calculation:** Average revenue per user × Number of users

#### How MRR Moves

| Movement | Impact |
|----------|--------|
| **Churn MRR** | Lost revenue (negative) |
| **Reactivation MRR** | Old users return (positive) |
| **Downgrade MRR** | Cheaper subscriptions (negative) |
| **Expansion MRR** | Upsells, more licenses (positive) |
| **New MRR** | New users (positive) |

---

### Net Revenue Retention (NRR)

Shows how much users value your product. Always expressed as percentage.

#### How NRR Works

- **100% NRR** — Retained all customers at same price
- **110% NRR** — Retained + some upsold (expansion > churn)
- **<100% NRR** — Business is decaying/shrinking

#### Why NRR Matters

- **Above 100%** — Revenue hockey sticks upward with new customers
- **Below 100%** — Revenue decaying, increases acquisition costs

**Benchmarks:** Best-in-class B2B enterprise SaaS: >125% NRR

---

### Gross Merchandise Value (GMV)

For marketplaces and payment providers only.

**Definition:** Sum of all purchases going through the intermediary.

**Useful for:** Indication of market share captured.

**Important:** Not applicable to other business types; not recognized revenue.

---

## The Profitability Funnel

### Funnel Levels

```
Revenue
    └── minus Cost of Revenue (COGS) = Gross Profit
            └── minus Acquisition Costs
                    └── minus Overheads = Profit
```

### Cost Types

| Type | Definition | Examples |
|------|------------|----------|
| **Variable costs** | Scale with customers/orders | Customer service, stock, payment fees, marketing |
| **Fixed costs** | Same regardless of size | Legal, accounting, office |

**Rule:** If you'd spend it with 0 customers, it's fixed. If only with more customers, it's variable.

---

### Gross Profit / Gross Margin

**Gross Profit** = Revenue - Cost of Revenue

**Gross Margin** = Gross Profit ÷ Revenue (as %)

**Example:**
- Revenue: $1M
- Cost of Revenue: $200K
- Gross Profit: $800K
- **Gross Margin: 80%**

#### What's in Cost of Revenue

- Royalty costs/fees
- Site hosting, software licenses
- Customer support/success teams
- Payment provider fees

#### Product's Role in Gross Margin

- Cut customer contacts
- Automate customer service
- Make upselling easier
- Reduce hosting/processing costs

---

## CLTV:CAC

### Customer Lifetime Value (CLTV)

Average revenue per customer, minus cost of revenue, for the time period customer stays.

**Types:**
- **Historic** — Actual value from past customers
- **Predictive** — Forecast based on retention rates

### Cost of Acquisition (CAC)

Average cost to acquire a customer (sales + marketing costs).

### The Ratio

**CLTV > CAC** = Business can profitably acquire users

**CLTV < CAC** = Losing money on each customer

---

### Common CLTV Mistakes

| Mistake | Problem |
|---------|---------|
| **Not enough data** | Early-stage companies lack stable metrics |
| **Long time periods** | B2C: payback <4 months. B2B: <24 months |
| **Wrong churn rate** | Use user churn, not revenue churn |
| **Not adjusting for costs** | Cost of revenue must show up somewhere |
| **Sample vs whole** | Small samples skew the picture |

---

### Better Alternative: Payback Windows

Monitor how long it takes for revenue to pay back acquisition costs.

**Benefits:**
- Helps optimize cash flow
- More actionable than theoretical CLTV
- Enables predictable investment cycles

---

### Why Product Cares About CAC

> "CAC can create a money-losing flywheel that starts at acquisition" — CJ Gustafson

**Product can reduce CAC via:**
- Virality / PLG loops
- Reducing cost of revenue
- Better product-market fit
- Improved activation and reduced churn

---

## Summary

### Retention Metrics

| Metric | Purpose |
|--------|---------|
| **Cohorts** | Track behavior over time by user group |
| **Gross Churn** | Users/revenue lost |
| **Net Churn** | Net growth/shrinkage |

### Income Metrics

| Metric | What It Measures |
|--------|------------------|
| **Revenue** | Recognized when service delivered |
| **Bookings** | Contracted future revenue |
| **Cash** | Actual money received |
| **ARR/MRR** | Subscription recurring revenue |
| **NRR** | Revenue retention + expansion |
| **GMV** | Marketplace transaction value |

### Profitability

| Level | Formula |
|-------|---------|
| **Gross Profit** | Revenue - Cost of Revenue |
| **Gross Margin** | Gross Profit ÷ Revenue |
| **Contribution** | Gross Profit - Acquisition Costs |
| **Profit** | Contribution - Overheads |

### Key Takeaways

1. **These are YOUR metrics** — Product is core driver of revenue/retention
2. **Agree on definitions** — Misalignment kills credibility
3. **Cohorts reveal truth** — Track user behavior over time
4. **NRR >100% = growth** — Below 100% means decay
5. **Gross margin matters** — Product can directly improve it
6. **CLTV:CAC is critical** — But watch payback windows
7. **Lagging indicators** — Actions today show up in months
