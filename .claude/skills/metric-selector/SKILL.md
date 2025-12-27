---
name: metric-selector
description: Selects appropriate success metrics for initiatives using the 5-lenses framework (Actionable, Accessible, Auditable, Aligned, Appropriate). Avoids vanity metrics and common traps. Use when choosing KPIs, defining success metrics, evaluating which metrics to track, or asking "what should we measure."
---

# Metric-Selector Utility

## Purpose

Selects appropriate success metrics for initiatives using the 5-lenses framework.

---

## Invocation

**Agent-called:** Typically called by Metrics agent

---

## Knowledge Folder

**Primary folder:** `knowledge/metrics/`

Search for "success metrics" or "choosing metrics" in this folder for detailed selection guidance and common traps. New files added to this folder are automatically available.

---

## 5-Step Selection Process

### Step 1: Define the Question
What are you trying to learn or prove?
- "Did this feature improve user engagement?"
- "Are we retaining customers better?"
- "Is this initiative worth continuing?"

### Step 2: Identify Candidates
List all metrics that could answer the question:
- Business metrics (revenue, churn, LTV)
- Product metrics (adoption, activation, engagement)
- User metrics (satisfaction, effort, completion)

### Step 3: Apply 5 Lenses
Evaluate each candidate metric through:

| Lens | Question |
|------|----------|
| **Actionable** | Can we influence this directly? |
| **Accessible** | Can we measure it reliably? |
| **Auditable** | Can we trust the data source? |
| **Aligned** | Does it connect to business outcomes? |
| **Appropriate** | Is it the right level of abstraction? |

### Step 4: Check for Traps
Common metric traps to avoid:
- **Vanity metrics** - Look good but don't matter
- **Lagging only** - No leading indicators
- **Proxy gone wrong** - Optimizing metric, not outcome
- **Too many metrics** - Diluted focus
- **Easy to game** - Can be manipulated

### Step 5: Define Measurement Plan
- Baseline: What's current state?
- Target: What success looks like?
- Timeline: When will we evaluate?
- Method: How will we measure?

---

## 5 Lenses Detail

### 1. Actionable
- Team can directly influence it
- Changes based on team's work
- Not dependent on external factors

### 2. Accessible
- Data is available
- Can be measured regularly
- Doesn't require months to see

### 3. Auditable
- Data source is reliable
- Calculation is clear
- Can verify accuracy

### 4. Aligned
- Connects to business outcomes
- Supports strategic goals
- Not disconnected from value

### 5. Appropriate
- Right granularity for the question
- Not too narrow or too broad
- Matches initiative scope

---

## Output Format

```
## Success Metric Selected
[Primary metric] - [Why this one]

## 5 Lenses Evaluation
- Actionable: [Yes/No] - [Explanation]
- Accessible: [Yes/No] - [Explanation]
- Auditable: [Yes/No] - [Explanation]
- Aligned: [Yes/No] - [Explanation]
- Appropriate: [Yes/No] - [Explanation]

## Measurement Plan
- Baseline: [Current value]
- Target: [Success threshold]
- Timeline: [When to evaluate]
- Method: [How to measure]

## Traps Avoided
[Which traps were considered and why this metric avoids them]
```

---

## Common Metric Traps

| Trap | Example | Fix |
|------|---------|-----|
| **Vanity** | Page views without engagement | Add depth metric |
| **Lagging only** | Only tracking revenue | Add leading indicators |
| **Proxy gaming** | Optimizing clicks not conversions | Measure true outcome |
| **Too many** | 20 KPIs for one initiative | Pick 1-3 that matter |
