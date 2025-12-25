# Choosing the Right Success Metrics

**Author:** Ed Biden (Hustle Badger)

**Source:** https://www.hustlebadger.com/metrics/success-metrics/

---

## Overview

A success metric is the yardstick you use to measure overall performance of your strategy, product, or feature. It's the single best quantifiable measure of how your product is doing over time.

**Definition breakdown:**
- **Single best** — Any metric alone is imperfect, but if you need one quick read, this is it
- **Quantifiable** — Something you can count and put a number on
- **Measure of performance** — A signal of how things are going
- **Over time** — It changes, enabling informed decisions

---

## Why Success Metrics Matter

| Benefit | Description |
|---------|-------------|
| **Clarify objective** | Pairing qualitative objective with quantitative measure |
| **Track performance** | Establish baseline and monitor changes over time |
| **Help prioritization** | Common currency to compare competing options |
| **Understand drivers** | See what creates impact |

---

## Leading vs. Lagging Metrics

**Lagging metrics** (revenue, profit, ARR, GMV):
- Direct business impact
- Delay between action and movement
- Difficult to see your team's impact

**Leading metrics** (engagement, conversion):
- More responsive to actions
- Clearer attribution
- Must still predict business impact

> The faster your metrics react, the quicker you can move. But if they don't predict business impact, they aren't useful.

**Goal:** Find a leading metric that's responsive AND a direct driver of lagging business metrics.

---

## 5 Steps to Define Your Success Metric

### 1. Business Metric

Identify the most important high-level business metric:
- Revenue
- Profit / EBITDA
- ARR (SaaS)
- GMV (Marketplaces)

**How to find it:**
- Ask leadership team
- Look at sales/marketing headline numbers
- Ask finance team

### 2. Mechanism

Write down WHY your feature is important. How will it move the business metric?

**Example — YunoJuno:**
> "We want to make it easier for clients to create and post briefs. Creating a brief is mandatory and the first step in booking a freelancer. More briefs → more bookings → more commission → more revenue."

**Brainstorm indicators:**
- Think through AARRR funnel (Acquisition, Activation, Retention, Referral, Revenue)
- Identify the core action where users get value

### 3. Definition

Design the actual metric using 5 lenses:

#### Lens 1: Correlation

Analyze which early indicators predict high-value customers (HVCs) vs. low-value customers (LVCs).

**Example findings:**
- Buy 1 item in 7 days: 75% HVCs vs 8% LVCs ✓ (strongest)
- 30x searches in 7 days: 78% HVCs vs 38% LVCs ✓
- Add 1 item to basket in 7 days: 84% HVCs vs 40% LVCs ✓

#### Lens 2: Position in Funnel

```
Leading ←────────────────────────→ Lagging
More traffic                   Less traffic

[Traffic] → [Searches] → [Product Page] → [Checkout] → [Revenue]
```

Start close to business metric, move up funnel only if you need more responsive/specific metrics.

#### Lens 3: Time Period

Balance stability vs. responsiveness:
- Daily = very responsive, very noisy
- 7-day average = somewhat noisy/responsive
- 14-day average = stable, lagging

**Rolling averages** often give best of both worlds.

#### Lens 4: Absolute vs. Relative

| Type | Shows | Hides |
|------|-------|-------|
| **Absolute** (revenue) | Overall scale | Per-user problems |
| **Relative** (revenue/user) | Per-user performance | Overall scale |

**Example — Udemy:**
- Success metric: Courses started (absolute)
- Health metrics: Courses per learner, Completion rate (relative)

#### Lens 5: Aggregate vs. Individual

Consider bucketing related activities if they deliver similar user value.

**Example — LinkedIn Newsfeed:**
- Individual: Likes, Comments, Reposts, Shares
- Aggregate: Social engagement = likes + comments + reposts + shares

### 4. Check

Validate your proposed metric:

| Check | Good Example | Bad Example |
|-------|--------------|-------------|
| **Intuitive** | % users who commented in 7 days | Complex multi-condition formula |
| **Measurable** | Sellers who sold 10+ items in 30 days | "Highly motivated sellers" |
| **Actionable** | Page load speed (lower = better) | Searches per user (higher or lower?) |
| **Influence** | Team-specific conversion rate | Company-wide revenue |

### 5. Iterate

Chart it and see what it tells you. Does it help you make decisions? If not, find a better alternative.

---

## Common Traps to Avoid

### 1. Vanity Metrics

Metrics that feel good but don't correlate with business success (pageviews, downloads, followers).

**Problem:** Focuses you on work that doesn't deliver meaningful impact.

### 2. Treating Metric as Goal

When you define objective as metric first, teams ignore strategy and move metric in any way possible.

**Result:** Dark patterns, or ignoring critical things that don't move the metric.

**Solution:** Remember metric is one indicator—keep reflecting on qualitative objective.

### 3. Noisy Metrics

If metric jumps around with no patterns, you get no indication of whether you're doing the right things.

**Solutions:**
- Increase duration
- Convert to relative number
- Go further up/down funnel

### 4. Failing to Move Metric

Some metrics are effectively constants.

**Diagnostic:**
- If shipping regularly AND other metrics moving → metric problem → find another
- If not shipping often AND no other movement → impact problem → more discovery needed

---

## Success Metric Examples

| Company | Success Metric |
|---------|----------------|
| **Notion** | % MAU using explanations once in past 7 days rolling |
| **GoCardless** | Monthly subscriber churn rate |
| **ASOS** | Average searches per user in past 7 days rolling |
| **Booking.com** | % Bookers using meal filter, 28 days rolling |

---

## Two Levels of Metrics

### Team Success Metric
Measures whether team is successful over medium term (quarter or year)

### Feature Success Metric
Measures whether individual feature is successful

Often the same, but sometimes more specific for features known to drive team metric.

---

## Summary

| Step | Purpose |
|------|---------|
| 1. Business metric | What you're ultimately trying to move |
| 2. Mechanism | How your actions move that metric |
| 3. Definition | 5 lenses to design precise metric |
| 4. Check | Intuitive, measurable, actionable, influenceable |
| 5. Iterate | Learn and improve over time |

### Key Takeaways

1. **Leading + predictive** — Find metrics that are responsive AND predict business impact
2. **Start at business metric** — Work up the funnel only as needed
3. **Use rolling averages** — Balance stability and responsiveness
4. **Pair absolute + relative** — Use health metrics for balance
5. **Correlation analysis** — Find what separates high-value from low-value customers
6. **Avoid vanity** — Make sure metrics actually drive business value
7. **Iterate** — First metric rarely perfect; learn and improve
