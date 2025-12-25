---
name: impact-model-builder
description: Creates driver trees connecting product activities to business outcomes. Maps north star metrics to drivers and leading indicators. Use when building impact models, creating driver trees, connecting metrics to business goals, or visualizing metric relationships.
---

# Impact-Model-Builder Utility

## Purpose

Creates driver trees that connect product activities to business outcomes.

---

## Invocation

**Agent-called:** Typically called by Metrics agent

---

## Knowledge Folder

**Primary folder:** `knowledge/metrics/`

Search for "impact" or "driver" in this folder for Ed Biden's complete 7-step process and examples. New files added to this folder are automatically available.

---

## What is an Impact Model?

A **driver tree** that maps:
- North Star Metric (what the business cares about)
- → Drivers (major factors that influence it)
- → Leading indicators (metrics teams can directly influence)

---

## 7-Step Process (Ed Biden)

### Step 1: Identify North Star
- Single metric representing business success
- Usually revenue, engagement, or growth-related
- Example: Monthly Active Revenue, DAU, GMV

### Step 2: Break into Drivers
- What components make up the North Star?
- Usually 2-4 major drivers
- Mathematical or causal relationship

### Step 3: Map Leading Indicators
- What team-controllable metrics predict each driver?
- Should be actionable and measurable
- Can be influenced within quarter

### Step 4: Assign Ownership
- Which team owns which branch?
- Company vs team level metrics
- Clear accountability

### Step 5: Identify Leverage Points
- Where does small change = big impact?
- Which indicators are underperforming?
- Where is effort best spent?

### Step 6: Set Targets
- Baseline for each metric
- Target improvement
- Realistic but ambitious

### Step 7: Review Cadence
- How often to check progress?
- When to revisit model assumptions?

---

## Driver Tree Structure

```
                    North Star Metric
                    (e.g., MRR Growth)
                           │
         ┌─────────────────┼─────────────────┐
         ▼                 ▼                 ▼
      Driver 1          Driver 2          Driver 3
   (New Revenue)     (Expansion)        (Retention)
         │                 │                 │
    ┌────┼────┐       ┌────┼────┐       ┌────┼────┐
    ▼    ▼    ▼       ▼    ▼    ▼       ▼    ▼    ▼
  Lead Lead Lead    Lead Lead Lead    Lead Lead Lead
  Ind  Ind  Ind     Ind  Ind  Ind     Ind  Ind  Ind
```

---

## Output Format

```
## North Star Metric
[Metric name] - [Current value] - [Target]

## Driver Tree

### Driver 1: [Name]
Relationship: [How it impacts North Star]
- Leading indicator 1.1: [Metric] - [Baseline] → [Target]
- Leading indicator 1.2: [Metric] - [Baseline] → [Target]
Owner: [Team]

### Driver 2: [Name]
Relationship: [How it impacts North Star]
- Leading indicator 2.1: [Metric] - [Baseline] → [Target]
- Leading indicator 2.2: [Metric] - [Baseline] → [Target]
Owner: [Team]

## Leverage Points
[Where to focus for maximum impact]

## Review Cadence
[How often to check and update]
```

---

## Company vs Team Level

| Level | Focus | Example |
|-------|-------|---------|
| **Company** | North Star, major drivers | MRR, Retention Rate |
| **Team** | Leading indicators they control | Feature adoption, Activation rate |

Teams should have metrics they can directly influence.
