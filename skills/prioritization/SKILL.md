---
name: prioritization
description: Use when comparing options, ranking features, deciding priorities, asking "what should we focus on," or when prioritization feels difficult.
---

# Prioritization

Helps teams prioritize at the right layer with the right criteria.

---

## Quick Start

1. Ask: "What are you trying to prioritize?"
2. Identify the layer (strategy, outcomes, opportunities, or solutions)
3. Check if foundations exist for that layer
4. Apply layer-appropriate prioritization
5. If still unclear after applying the right framework, the problem is one layer up

---

## Knowledge Access

See `## prioritization` in `resources.md`. Read Core first (especially layered-prioritization.md and confidence-not-value.md).

---

## Core Principle

> "Prioritize based on value" is bad advice. Value is contextual. Without vision, strategy, and metrics, you have no criteria for comparison.

Most prioritization problems are actually **strategy problems** in disguise.

---

## The Layered Model

Prioritization happens at four layers. Each has different criteria.

```
LAYER              WHAT YOU'RE PRIORITIZING     THE QUESTION
────────────────────────────────────────────────────────────────
Strategy           Where to compete             "Which path forward?"
       ↓
Outcomes           Which problems to solve      "What enables our strategy?"
       ↓
Opportunities      Which user needs to address  "What problems matter most?"
       ↓
Solutions          Which approach to take       "How do we solve this?"
```

**Don't apply solution frameworks (RICE, VEUC) to strategy problems.**

---

## Identifying the Layer

When user asks for help prioritizing, first identify what they're prioritizing:

| User Says | They're Prioritizing | Layer |
|-----------|----------------------|-------|
| "Should we go upmarket or expand features?" | Direction | Strategy |
| "Which problem should we solve first?" | Problems/goals | Outcomes |
| "Which user need matters more?" | User needs | Opportunities |
| "Feature A or Feature B?" | Approaches | Solutions |
| "What should our team focus on?" | Could be any | Ask to clarify |

Ask: "Are you trying to decide **where to focus** (strategy), **what problem to solve** (outcomes/opportunities), or **how to solve it** (solutions)?"

---

## Prioritization by Layer

### Strategy Layer

**Question:** Where should we compete? Which direction?

**Criteria:**
- Vision alignment (does this move toward our north star?)
- Market opportunity (is this a winnable game?)
- Competitive advantage (can we be differentiated here?)
- Capability fit (do we have or can we build what's needed?)

**Not useful here:** RICE, effort estimation, user reach numbers

**If unclear:** Go to `strategy` skill

---

### Outcomes Layer

**Question:** Which problems/outcomes should we focus on?

**Criteria:**
- Strategic enablement (does solving this unlock strategy?)
- Blocking factor (does NOT solving this prevent strategy?)
- Metric impact (does this move key metrics?)
- Dependency awareness (what must come first?)

**Not useful here:** Feature comparisons, user feature requests

**If unclear:** Check if strategy is defined. If not, go to `strategy` skill.

---

### Opportunities Layer

**Question:** Which user needs should we address?

**Criteria:**
- Strategic alignment (gets you closer to goals, not just high reach)
- Problem significance (how painful for users?)
- Opportunity sizing (how many users, how often?)
- Market factors (competitive differentiation potential)

**Critical insight from Ant Murphy:** "Valuable opportunities are the ones that get you closer to your goals and strategy, not the ones with the highest reach."

High-reach complaints are not automatically high-priority opportunities.

**Not useful here:** Solution comparisons, effort estimation (effort belongs in solution phase)

**If unclear:** Check if outcomes are defined. If not, go to `metrics` or `discovery` skill.

---

### Solutions Layer

**Question:** Which approach should we take?

**This is where frameworks like DHM, VEUC, RICE belong.**

**Criteria:**
- Opportunity fit (does it actually solve the prioritized opportunity?)
- Confidence (how sure are we this works?)
- Effort/complexity
- Risk profile

**Frameworks to apply:**
- **DHM** (Gibson Biddle): Delight, Hard-to-copy, Margin-enhancing
- **VEUC** (Ant Murphy): Value, Effort, Urgency, Confidence
- **Confidence-weighted** (Ant Murphy): Prioritize by confidence, not abstract value

**If unclear:** Check if opportunity is well-defined. If not, go back to opportunity layer.

---

## The Confidence Lens

At every layer, reframe "What's most valuable?" to:

**"What do we have most confidence in?"**

| Layer | Value Question (Vague) | Confidence Question (Actionable) |
|-------|------------------------|----------------------------------|
| Strategy | "Which strategy is most valuable?" | "How confident are we this is the right path?" |
| Outcomes | "Which outcome has most value?" | "How confident are we this outcome matters?" |
| Opportunities | "Which opportunity is most valuable?" | "How confident are we this is a real problem?" |
| Solutions | "Which solution delivers most value?" | "How confident are we this solves it?" |

**Low confidence doesn't mean deprioritize. It means discover first.**

```
High confidence + High impact → Build
High confidence + Low impact  → Maybe later
Low confidence + High impact  → Discover first
Low confidence + Low impact   → Skip
```

---

## Foundation Check

Before prioritizing, verify foundations exist for that layer:

```
Prioritizing...    Requires...
─────────────────────────────────────────
Strategy           Vision
Outcomes           Vision + Strategy
Opportunities      Vision + Strategy + Metrics
Solutions          Vision + Strategy + Metrics + Opportunities
```

**If foundation is missing:**

1. Note what's missing and why it matters
2. Offer to build it: "We need [X] before prioritizing [Y]. Want to work on that first?"
3. If user insists on skipping, proceed but flag gaps explicitly

---

## When Prioritization Stays Difficult

If prioritization remains unclear after applying the right layer's criteria:

1. **The options are basically the same** - When it's truly hard to decide, the options often have similar expected value. Pick one and move.

2. **Missing foundation** - Check one layer up. No strategy = no criteria for prioritization.

3. **Wrong layer** - You might be applying solution frameworks to an outcome problem.

4. **Need more confidence** - Route to discovery instead of forcing a decision.

---

## Output Format

```markdown
## Prioritization Assessment

### Layer Identified
[Strategy / Outcomes / Opportunities / Solutions]

### Foundation Check
[What exists, what's missing]

### Criteria Applied
[Which criteria from this layer]

### Recommendation
[What to prioritize and why]

### Confidence Level
[High/Medium/Low - what would increase it]

### What We're NOT Doing
[Trade-offs acknowledged]
```

---

## Anti-patterns

| Pattern | Why It Fails | Fix |
|---------|--------------|-----|
| RICE for everything | RICE is for solutions, not strategy | Identify the layer first |
| Prioritizing by reach | High reach is not high priority | Check strategic alignment |
| Effort estimation too early | Effort belongs in solution phase | Separate opportunity from solution |
| Debating value without strategy | No shared criteria | Define strategy first |
| Forcing decisions with low confidence | Premature commitment | Route to discovery |

---

## Routing to Other Skills

| Situation | Route To |
|-----------|----------|
| No vision defined | `vision` skill |
| No strategy defined | `strategy` skill |
| No metrics defined | `metrics` skill |
| No opportunities mapped | `discovery` skill |
| Ready to plan what to build | `roadmap` skill |
| Need to validate an opportunity | `discovery` skill |
