---
name: metrics
description: Use when discussing metrics, OKRs, KPIs, success measurement, leading indicators, or "how do we know if this works."
---

# Metrics

Defines and organizes success measurement. Focuses on connecting metrics to outcomes, building impact models, and selecting appropriate success indicators.

---

## Quick Start

1. Check `context/vision.md` and `context/strategy.md` exist (metrics need strategic context)
2. Start with the outcome you want to achieve
3. Identify leading indicators that predict that outcome
4. Choose metrics that are actionable (team can influence)
5. See `## Metrics` in `resources.md` for knowledge (Core first, Additional as needed)

---

## Core Purpose

**Metrics answers:**
- How do we know if we're succeeding?
- What should we measure?
- How do leading indicators connect to business outcomes?
- Should we use OKRs (and when)?

**Metrics is NOT:**
- Data analysis execution (this is strategic metric design)
- Dashboard building (focuses on what to measure, not how)
- Quarterly planning

---

## Key Responsibilities

1. **Impact Model Design** - Build driver trees connecting activities to outcomes
2. **Metric Selection** - Choose right success metrics for initiatives
3. **Leading/Lagging Mapping** - Connect leading indicators to lagging outcomes
4. **OKR Guidance** - Help formulate OKRs (when appropriate)

---

## Core Concepts

- Leading indicators = predictive, actionable (activation rate, feature adoption)
- Lagging indicators = outcomes, delayed (revenue, churn)
- Goal: Find leading indicators that predict lagging outcomes

---

## Output Format

**Before creating any output:** Follow the base rule in CLAUDE.md - summarize sections, ask permission, then save.

**Primary artifact:** Metric framework for initiative

```
## Success Metric
[Primary metric that indicates success]

## Leading Indicators
- [Indicator 1] - [Relationship to success metric]
- [Indicator 2] - [Relationship to success metric]

## Lagging Outcomes
- [Business outcome this ladders up to]

## Measurement Plan
- [How will we track these?]
- [What's our baseline?]
- [What's our target?]
```

---

## Success Criteria

1. Metrics connected to business outcomes
2. Leading indicators identified and actionable
3. Appropriate framework for company stage (OKRs optional)
4. Clear measurement plan
5. Metrics are outcomes, not outputs

---

## Common Pitfalls

1. **Output metrics** - Measuring what we shipped vs impact
2. **Vanity metrics** - Looks good but doesn't matter
3. **Too many metrics** - Focus on 1-3 that matter most
4. **Forcing OKRs** - Not every stage needs quarterly OKRs
5. **Missing leading indicators** - Only tracking lagging outcomes

---

## Verification Criteria

Before presenting metrics deliverable, run these checks. Maximum 3 regeneration attempts per failed check.

### Foundation Prerequisites

**Check before creating metrics:**
- [ ] **Vision exists** - context/vision.md must exist
- [ ] **Strategy exists** - context/strategy.md must exist

**If missing:** Warn user and recommend building foundation first. User can override and proceed with gaps.

### Structural Requirements

**Core Components:**
- [ ] **Success Metric defined** - Primary metric clearly stated
- [ ] **Leading Indicators present** - At least 1-2 leading indicators identified
- [ ] **Lagging Outcomes stated** - Business outcomes this ladders up to
- [ ] **Measurement Plan exists** - Includes how to track, baseline, and target
- [ ] **Saved to context** - Saved to `context/metrics.md` or appropriate context file

### Quality Checks

**Strategic Alignment:**
- [ ] **Connected to strategy** - References or builds from strategy in context/strategy.md
- [ ] **Aligned with vision** - Metrics support the product vision
- [ ] **Ladder to business outcomes** - Clear chain from metric to business impact

**Metric Design:**
- [ ] **Outcomes not outputs** - Measures impact, not what was shipped (e.g., "activation rate" not "features shipped")
- [ ] **Actionable** - Team can actually influence these metrics
- [ ] **Measurable** - Can actually be tracked with available data
- [ ] **Focused** - 1-3 key metrics maximum, not a laundry list
- [ ] **Not vanity metrics** - Metrics that actually indicate success, not just "looks good"

**Leading/Lagging Relationship:**
- [ ] **Relationship is clear** - Each leading indicator explicitly states how it predicts the outcome
- [ ] **Leading indicators are actually leading** - Predictive and occur before the outcome
- [ ] **Lagging indicators are actual outcomes** - Business results, not intermediate steps

**Measurement Plan:**
- [ ] **Baseline stated** - Current state is known or estimated
- [ ] **Target is realistic** - Goal is ambitious but achievable
- [ ] **Tracking method clear** - Team knows how they'll measure this

**OKR-Specific (if using OKRs):**
- [ ] **Objective is qualitative** - Inspiring direction, not metric
- [ ] **Key Results are quantitative** - Specific numbers with targets
- [ ] **2-5 Key Results per Objective** - Not too few, not too many
- [ ] **Stretch goals** - Ambitious (60-70% confidence), not guaranteed wins

### Verification Process

1. Generate draft metrics framework
2. Run all checks above
3. For each failed check:
   - **Can we fix with context we have?** → Regenerate silently
   - **Need user input?** → Ask specific question, then regenerate
4. Show progress: "Checking [criterion]... ✓ or ✗ [reason]"
5. Maximum 3 attempts per check
6. If still failing after 3 attempts → Proceed with warning: "⚠ Could not verify [criterion] after 3 attempts"
7. Present metrics with Eval Summary appended

### Eval Summary Format

Append to metrics deliverable:

```markdown
---
## Eval Summary

### Foundation Prerequisites
- [✓] Vision exists
- [✓] Strategy exists

### Structural Requirements
- [✓] Success Metric defined
- [✓] Leading Indicators present (2 identified)
- [✓] Lagging Outcomes stated
- [✓] Measurement Plan exists
- [✓] Saved to context

### Quality Checks - Strategic Alignment
- [✓] Connected to strategy
- [✓] Aligned with vision
- [✓] Ladder to business outcomes

### Quality Checks - Metric Design
- [✓] Outcomes not outputs
- [✓] Actionable
- [✓] Measurable
- [✓] Focused (3 metrics)
- [✓] Not vanity metrics

### Quality Checks - Leading/Lagging Relationship
- [✓] Relationship is clear
- [✓] Leading indicators are actually leading
- [✓] Lagging indicators are actual outcomes

### Quality Checks - Measurement Plan
- [✓] Baseline stated
- [✓] Target is realistic
- [✓] Tracking method clear

### OKR-Specific (if applicable)
- [ ] Not using OKRs for this deliverable
```

If using OKRs, replace last section with:
```markdown
### OKR-Specific Checks
- [✓] Objective is qualitative
- [✓] Key Results are quantitative
- [✓] 2-5 Key Results per Objective (3 KRs)
- [✓] Stretch goals (70% confidence)
```

Use:
- `[✓]` for passed checks
- `[✗]` for failed checks (with reason)
- `[ ]` for not applicable (with reason)
