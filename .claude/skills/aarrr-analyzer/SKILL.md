---
name: aarrr-analyzer
description: Analyzes product metrics through the AARRR pirate funnel (Acquisition, Activation, Retention, Revenue, Referral). Identifies bottlenecks and stage-appropriate metrics. Use when analyzing funnels, diagnosing growth problems, reviewing pirate metrics, or asking "where is our funnel breaking."
---

# AARRR-Analyzer Utility

## Purpose

Analyzes product metrics through the AARRR pirate funnel to identify bottlenecks.

---

## Invocation

**Agent-called:** Typically called by Metrics agent

---

## Knowledge Folder

**Primary folder:** `knowledge/metrics/`

Search for "AARRR" or "funnel" in this folder for detailed acquisition, activation, retention, revenue, and referral metrics. New files added to this folder are automatically available.

---

## AARRR Funnel Overview

```
Acquisition → Activation → Retention → Revenue → Referral
```

| Stage | Question | Focus |
|-------|----------|-------|
| **Acquisition** | How do users find us? | Channels, traffic |
| **Activation** | Do they have a good first experience? | Onboarding, aha moment |
| **Retention** | Do they come back? | Engagement, stickiness |
| **Revenue** | How do they pay us? | Conversion, ARPU |
| **Referral** | Do they tell others? | Virality, NPS |

---

## Stage-by-Stage Analysis

### Acquisition
**Question:** How do users find us?

| Metric | What It Measures |
|--------|-----------------|
| Traffic by channel | Where users come from |
| CAC by channel | Cost to acquire |
| Sign-up rate | Traffic → Sign-up conversion |
| Channel mix | Diversity of acquisition |

**Key insight:** Which channels are efficient and scalable?

### Activation
**Question:** Do users have a good first experience?

| Metric | What It Measures |
|--------|-----------------|
| Activation rate | % completing key action |
| Time to activate | How fast users get value |
| Onboarding completion | % finishing setup |
| Aha moment rate | % experiencing core value |

**Key insight:** Are users finding value quickly?

### Retention
**Question:** Do users come back?

| Metric | What It Measures |
|--------|-----------------|
| DAU/MAU ratio | Daily engagement stickiness |
| Cohort retention | % returning by time period |
| Churn rate | % leaving each period |
| Feature retention | Which features drive return |

**Key insight:** Is the product creating habit?

### Revenue
**Question:** How do users pay us?

| Metric | What It Measures |
|--------|-----------------|
| Conversion rate | Free → Paid |
| ARPU/ARPA | Revenue per user/account |
| LTV | Lifetime value |
| LTV:CAC ratio | Unit economics health |
| Expansion revenue | Upsell/cross-sell success |

**Key insight:** Is the business model working?

### Referral
**Question:** Do users tell others?

| Metric | What It Measures |
|--------|-----------------|
| NPS | Likelihood to recommend |
| Viral coefficient | Users brought by each user |
| Referral rate | % using referral features |
| Organic traffic % | Word-of-mouth growth |

**Key insight:** Is growth compounding?

---

## Funnel Analysis Process

### Step 1: Map Current Metrics
- What do you measure at each stage?
- Where are the gaps?

### Step 2: Identify Bottleneck
- Where is the biggest drop-off?
- Which stage is underperforming?

### Step 3: Diagnose Root Cause
- Why is this stage struggling?
- What evidence supports this?

### Step 4: Prioritize Improvement
- Which stage has highest leverage?
- Where will improvement compound?

---

## Output Format

```
## Funnel Overview

| Stage | Key Metric | Current | Target | Status |
|-------|------------|---------|--------|--------|
| Acquisition | [metric] | [value] | [target] | [Red/Yellow/Green] |
| Activation | [metric] | [value] | [target] | [Red/Yellow/Green] |
| Retention | [metric] | [value] | [target] | [Red/Yellow/Green] |
| Revenue | [metric] | [value] | [target] | [Red/Yellow/Green] |
| Referral | [metric] | [value] | [target] | [Red/Yellow/Green] |

## Bottleneck Analysis
Stage: [Which stage]
Drop-off: [From X% to Y%]
Root cause hypothesis: [What's causing it]

## Recommended Focus
[Which stage to prioritize and why]

## Metrics Gaps
[What we're not measuring but should]
```

---

## Common AARRR Mistakes

1. **Optimizing wrong stage** - Fix activation before scaling acquisition
2. **Ignoring retention** - Leaky bucket problem
3. **Revenue-only focus** - Missing leading indicators
4. **Forgetting referral** - Missing compound growth
