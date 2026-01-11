---
name: strategy
description: Use when discussing strategy, positioning, differentiation, competitive advantage, "how to win," or prioritization feels unclear.
---

# Strategy

Defines how to win in the market. Works through three interconnected patterns: why this opportunity (Narrative), where we compete (Playing Field), and how we position to win (Winning Moves).

---

## Quick Start

1. Check `context/vision.md` exists (if not, build foundation first)
2. Identify which pattern needs work: Narrative, Playing Field, or Winning Moves
3. Apply the "Does this help us say NO?" test
4. See `## Strategy` in `resources.md` for knowledge (Core first, Additional as needed)

---

## Core Purpose

**Strategy answers:**
- How will we win?
- What choices will we make (and NOT make)?
- Where will we focus?
- What advantages will we build?

**Strategy is NOT:**
- Vision (see `vision` skill)
- Roadmap (see `roadmap` skill)
- Execution plan

---

## Quick Reference

```
STRATEGIC NARRATIVE  →  Why this market opportunity?
PLAYING FIELD        →  Where do we compete?
WINNING MOVES        →  How do we position to win?

TEST: Does this help us say NO?
```

See `knowledge/strategy/product-strategy-patterns-herbig.md` for detailed framework with connections.

---

## Key Responsibilities

1. **Strategic Choices** - Define where to play, how to win, what to prioritize
2. **Framework Application** - Apply DHM, Four Fits, and other strategic frameworks
3. **Strategy Validation** - Test if strategy is decisive, differentiated, feasible
4. **Trade-off Articulation** - Make explicit what we're NOT doing

---

## Output Format

**Primary artifact:** Strategy document structured by patterns

```
## Strategic Narrative (Why)
**Vision:** [Future state for users]
**North Star:** [1-3 metrics that define winning]

**Market Reality:** [What's happening in the market that creates opportunity?]
**Our Hypothesis:** [What do we believe that others don't?]
**Urgency:** [Why must we act now? What's the window?]
**Conviction:** [Why will customers choose us over alternatives?]

## Playing Field (Where)
**Audiences:** [Who we're building for]
**Jobs:** [Progress they care about]
**Alternatives:** [What we're compared against]

## Winning Moves (How)
**Segments:** [Which customers get priority]
**Value Props:** [What value we deliver]
**Channels:** [How we reach them]
**Differentiators:** [What makes us hard-to-copy]
**Trade-offs:** [What we're NOT doing]

## Risks & Mitigation

| Risk Category | Example Risk | Impact | Mitigation Strategy |
|---------------|--------------|--------|---------------------|
| [Category]    | [Specific risk] | [What happens if this occurs] | [How we'll address it] |

## Validation
Does this strategy help us say NO? [Yes/No + evidence]
```

---

## Success Criteria

1. **Decisive** - Strategy helps team say NO clearly
2. **Differentiated** - Strategy is distinct from alternatives
3. **Actionable** - Teams can derive decisions from it
4. **Aligned** - All three patterns reinforce each other
5. **Focused** - Clear choices, not a list of everything

---

## Common Pitfalls

1. **Indecisive strategy** - Trying to do everything, no clear focus
2. **Me-too strategy** - Copying competitors without differentiation
3. **Feature list strategy** - Confusing tactics with strategy
4. **Vague platitudes** - "Be customer-focused" without specifics
5. **Mismatched work type** - Growth work when need PMF work

---

## Verification Criteria

Before presenting strategy deliverable, run these checks. Maximum 3 regeneration attempts per failed check.

### Foundation Prerequisites

**Check before creating strategy:**
- [ ] **Vision exists** - context/vision.md must exist

**If missing:** Warn user and recommend building vision first. User can override and proceed with gaps.

### Structural Requirements

**Pattern Completeness:**
- [ ] **All three patterns present** - Strategic Narrative, Playing Field, Winning Moves sections exist
- [ ] **Strategic Narrative complete** - Includes Vision, North Star, Market Reality, Hypothesis, Urgency, Conviction (all 6 elements)
- [ ] **Playing Field complete** - Includes Audiences, Jobs, Alternatives
- [ ] **Winning Moves complete** - Includes Segments, Value Props, Channels, Differentiators, Trade-offs

**Required Sections:**
- [ ] **Risks & Mitigation table** - Table with Risk Category, Example Risk, Impact, Mitigation Strategy (minimum 3 risks)
- [ ] **Validation section** - Includes "Does this help us say NO?" with answer and evidence
- [ ] **Trade-offs explicit** - "What we're NOT doing" is clearly stated in Winning Moves

**Context Linkage:**
- [ ] **Vision linkage** - References or builds from vision in context/vision.md
- [ ] **Saved to context** - Saved to `context/strategy.md`

### Quality Checks

**Boundaries:**
- [ ] **Breadth defined** - Clear scope (one product, product line, or portfolio)
- [ ] **Time horizon stated** - Explicit timeframe (e.g., "next 12 months", "3-year strategy")

**Alignment:**
- [ ] **Acknowledges constraints** - References business, tech, or market constraints that shape choices
- [ ] **Coherent across patterns** - Strategic Narrative, Playing Field, and Winning Moves reinforce each other (not contradictory)

**Informed by Data:**
- [ ] **Market Reality is factual** - Verifiable market conditions, not opinions or assumptions
- [ ] **Data-backed claims** - Key assertions reference data sources or research (even if informal)

**Measurable:**
- [ ] **North Star is measurable** - Metric can actually be tracked
- [ ] **Success criteria clear** - Can determine if strategy is working

**Detailed and Actionable:**
- [ ] **Explains WHY** - Rationale for choices is clear (not just WHAT was chosen)
- [ ] **Specific, not vague** - Concrete choices, not platitudes like "be customer-focused"
- [ ] **Teams can act on it** - Specific enough to guide roadmap decisions

**Strategic Choice Tests:**
- [ ] **Says NO effectively** - Test: Can this strategy clearly reject a plausible adjacent initiative? If unclear, strategy lacks focus
- [ ] **Passes "opposite of stupid" test** - For each major choice: is the opposite a valid alternative (not obviously bad)? If opposite is stupid, it's not a real choice
- [ ] **Hypothesis is contrarian** - States a belief others don't hold (not "AI is important" but "AI agents can automate 85% of workflows")
- [ ] **Urgency creates focus** - Specific time window or reason for urgency, not vague "eventually"

**Differentiation:**
- [ ] **Decisive** - Makes clear choices, not trying to do everything
- [ ] **Differentiated** - Distinct from "copy what competitors do"
- [ ] **Conviction is testable** - "Why we'll win" can be validated with customer evidence

### Verification Process

1. Generate draft strategy document
2. Run all checks above
3. For each failed check:
   - **Can we fix with context we have?** → Regenerate silently
   - **Need user input?** → Ask specific question, then regenerate
4. Show progress: "Checking [criterion]... ✓ or ✗ [reason]"
5. Maximum 3 attempts per check
6. If still failing after 3 attempts → Proceed with warning: "⚠ Could not verify [criterion] after 3 attempts"
7. Present strategy with Eval Summary appended

### Eval Summary Format

Append to `context/strategy.md` and any strategy deliverable:

```markdown
---
## Eval Summary

### Foundation Prerequisites
- [✓] Vision exists

### Structural Requirements
- [✓] All three patterns present
- [✓] Strategic Narrative complete (all 6 elements)
- [✓] Playing Field complete
- [✓] Winning Moves complete
- [✓] Risks & Mitigation table (4 risks identified)
- [✓] Validation section included
- [✓] Trade-offs explicit
- [✓] Vision linkage verified
- [✓] Saved to context

### Quality Checks
- [✓] Breadth defined (product line level)
- [✓] Time horizon stated (12 months)
- [✓] Acknowledges constraints (tech debt limits scope)
- [✓] Coherent across patterns
- [✓] Market Reality is factual
- [✓] Data-backed claims
- [✓] North Star is measurable
- [✓] Success criteria clear
- [✓] Explains WHY choices made
- [✓] Specific, not vague
- [✓] Teams can act on it
- [✓] Says NO effectively
- [✓] Passes "opposite of stupid" test
- [✓] Hypothesis is contrarian
- [✓] Urgency creates focus
- [✓] Decisive (clear choices)
- [✓] Differentiated
- [✗] Conviction is testable - Need customer validation evidence after 3 attempts
```

Use:
- `[✓]` for passed checks
- `[✗]` for failed checks (with reason)
- `[ ]` for not applicable (with reason)
