---
name: opportunity-tree
description: Creates and prioritizes Opportunity Solution Trees (OST) using Teresa Torres' framework. Maps customer opportunities to outcomes and solutions. Use when organizing discovery findings, structuring opportunities, deciding which problem to solve, or building an OST.
---

# Opportunity-Tree Utility

## Purpose

Creates and prioritizes Opportunity Solution Trees (OST) using Teresa Torres' framework.

---

## Invocation

**Agent-called:** Typically called by Discovery agent

---

## Knowledge Folder

**Primary folder:** `knowledge/discovery/`

Search for "opportunity" or "OST" in this folder for Teresa Torres' complete framework and prioritization guidance. New files added to this folder are automatically available.

---

## OST Structure

```
        Desired Outcome (Business/Product)
                    │
        ┌───────────┼───────────┐
        ▼           ▼           ▼
   Opportunity  Opportunity  Opportunity
   (Customer    (Customer    (Customer
    need 1)      need 2)      need 3)
        │           │           │
    ┌───┼───┐   ┌───┼───┐   ┌───┼───┐
    ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼   ▼
   Sol Sol Sol Sol Sol Sol Sol Sol Sol
```

---

## 3-Step Prioritization Process

### Step 1: Discover Opportunities
- Talk to customers weekly
- Frame in customer language (not solution language)
- Ask about needs, not feature requests

### Step 2: Map to Tree
- Connect opportunities to desired outcome
- Group related opportunities
- Identify parent-child relationships

### Step 3: Prioritize Opportunities (Not Solutions)
Questions to ask:
- Which opportunity, if addressed, would have the biggest impact on our outcome?
- Which opportunity do we have the most confidence we can address?
- Which is most aligned with our strategy?

---

## Key Principles

### Use Customer Language
| Bad (Solution) | Good (Opportunity) |
|----------------|-------------------|
| "Add export feature" | "I need to share reports with my team" |
| "Build mobile app" | "I need to check status while away from desk" |

### Two-Way Door Decisions
- Most opportunity choices are reversible
- Don't over-analyze - pick and learn
- Save deep analysis for one-way doors

### Prioritize Opportunities, Not Solutions
- Choose which problem to solve
- Then explore multiple solutions
- Don't jump to "build feature X"

---

## Output Format

```
## Desired Outcome
[Business/product outcome we're targeting]

## Opportunity Tree

### Opportunity 1: [Customer language framing]
- Evidence: [Research/data supporting this]
- Impact potential: [High/Medium/Low]
- Confidence: [High/Medium/Low]

### Opportunity 2: [Customer language framing]
- Evidence: [Research/data supporting this]
- Impact potential: [High/Medium/Low]
- Confidence: [High/Medium/Low]

## Priority Recommendation
[Which opportunity to pursue first and why]

## Decision Type
[One-way door (needs more analysis) / Two-way door (safe to proceed)]
```

---

## When to Use

- After customer research yields multiple potential directions
- When team is debating which problem to solve
- To structure discovery findings
- Before committing to solution design
