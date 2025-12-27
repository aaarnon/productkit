---
name: prioritization
description: Applies prioritization frameworks (VEUC, DHM, Can Do vs Should Do) to help decide what to work on. Use when comparing options, ranking features, deciding priorities, or when someone asks "what should we focus on" or "how do we prioritize this."
---

# Prioritization Utility

## Purpose

Applies structured prioritization frameworks when priorities aren't obvious.

---

## Invocation

**Hybrid:** Can be called by user directly or by agents (Strategy, Discovery, Roadmap)

---

## Knowledge Folder

**Primary folder:** `knowledge/prioritization/`

Search this folder for deeper content on VEUC framework, decision-making approaches, and prioritization philosophy. New files added to this folder are automatically available.

---

## Core Principle

> "If priority isn't obvious, you have a strategy problem."

Most prioritization frameworks (RICE, MoSCoW, Kano) are useless because **when it's difficult to decide, the options are basically the same.**

Results are distributed **logarithmically** - some things give 100x impact, one item often delivers more than everything else combined.

---

## Key Frameworks

### Focus Test
If it's not blindingly obvious what's most valuable:
- You don't understand users/needs well enough
- Focus on 2-3 core user needs, 1-2 core channels

### DHM Assessment
| Dimension | Question |
|-----------|----------|
| **Delight** | How does this delight customers? |
| **Hard-to-copy** | Does this build lasting advantages? |
| **Margin-enhancing** | How does this deliver business value? |

### VEUC Framework
| Factor | Weight |
|--------|--------|
| **Value** | Impact on users/business |
| **Effort** | Time/resources required |
| **Urgency** | Time sensitivity |
| **Confidence** | How sure are we? |

### Work Type by Stage
| Stage | Prioritize |
|-------|------------|
| **Pre-PMF** | Feature work |
| **Scaling** | Growth work |
| **Bottlenecked** | Scaling work |
| **Expansion** | PMF expansion work |

### Can Do vs Should Do
```
        Can Do
        High │ Low
       ┌─────┼─────┐
Should │  DO │ GET │
Do High│     │HELP │
       ├─────┼─────┤
Should │MAYBE│KILL │
Do Low │     │     │
       └─────┴─────┘
```

---

## Output Format

```
## Priority Recommendation
[What to prioritize and why]

## Framework Applied
[Which framework, why it fits]

## Trade-offs
[What we're NOT doing and why that's okay]

## Confidence
[How confident, what would change this]
```

---

## When to Escalate

If prioritization remains unclear after applying frameworks:
→ **Strategy problem** - Suggest calling Strategy agent
