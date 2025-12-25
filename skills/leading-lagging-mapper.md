---
name: leading-lagging-mapper
description: Maps relationships between leading indicators and lagging outcomes. Creates indicator chains showing how actionable metrics predict business results. Use when connecting metrics, understanding indicator relationships, building metric chains, or asking "what predicts this outcome."
---

# Leading-Lagging-Mapper Utility

## Purpose

Maps relationships between leading indicators and lagging outcomes to identify predictive metrics.

---

## Invocation

**Agent-called:** Typically called by Metrics agent

---

## Knowledge Folder

**Primary folder:** `knowledge/metrics/`

Search for "leading" or "lagging" in this folder for detailed indicator relationships and AARRR funnel metrics. New files added to this folder are automatically available.

---

## Leading vs Lagging Indicators

| Type | Characteristics | When to Use |
|------|-----------------|-------------|
| **Leading** | Predictive, actionable, controllable | Daily/weekly decisions |
| **Lagging** | Outcome, business result, delayed | Quarterly/annual review |

**Goal:** Find leading indicators that reliably predict lagging outcomes.

---

## Mapping Framework

### Step 1: Identify Lagging Outcomes
What business results matter?
- Revenue (ARR, MRR, GMV)
- Retention (Churn, NRR, Cohort retention)
- Growth (User growth, market share)

### Step 2: Hypothesize Leading Indicators
What activities/behaviors predict those outcomes?
- User engagement metrics
- Feature adoption metrics
- Activation metrics

### Step 3: Validate Relationships
- Does leading indicator actually correlate with lagging outcome?
- What's the time lag?
- How strong is the relationship?

### Step 4: Define the Chain
```
Leading → Intermediate → Lagging
```

---

## Common Indicator Chains

### Acquisition Chain
```
Traffic → Sign-ups → Activated Users → Paying Customers
(Leading)  (Leading)    (Leading)        (Lagging)
```

### Retention Chain
```
Feature Usage → Engagement Score → Renewal → Revenue Retention
(Leading)        (Leading)        (Lagging)   (Lagging)
```

### Expansion Chain
```
Product Qualified → Upsell Opportunity → Expansion Revenue
(Leading)           (Leading)            (Lagging)
```

---

## Time-Lag Considerations

| Metric Type | Typical Lag | Use For |
|-------------|-------------|---------|
| **Daily/Weekly** | Same day | Operational decisions |
| **Monthly** | 2-4 weeks | Tactical adjustments |
| **Quarterly** | 1-3 months | Strategic review |
| **Annual** | 6-12 months | Long-term strategy |

Early indicators with shorter lags enable faster learning and adjustment.

---

## Output Format

```
## Lagging Outcome
[Business metric we care about]

## Indicator Chain

### Leading Indicators (Actionable)
1. [Metric] - [Time to impact] - [Relationship strength]
2. [Metric] - [Time to impact] - [Relationship strength]

### Intermediate Indicators
1. [Metric] - [Time to impact] - [Relationship strength]

### Lagging Outcomes (Business Results)
1. [Metric] - [Measurement frequency]

## Visualization
[Leading 1] → [Leading 2] → [Intermediate] → [Lagging]
    │              │              │              │
  Days           Weeks         Months       Quarters

## Validation Status
[Hypothesized / Validated with data]
```

---

## Cohort Analysis Guidance

For retention metrics, analyze by cohort:
- Group users by signup date/quarter
- Track behavior over time
- Compare cohorts to understand trends
- Identify which leading indicators correlate with retention
