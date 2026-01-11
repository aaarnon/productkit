---
name: roadmap
description: Use when discussing roadmap, initiative planning, prioritization, "what to build when," or roadmap communication.
---

# Roadmap

Plans and communicates product initiatives. Focuses on initiative sequencing, storytelling, and creating artifacts that align teams and stakeholders.

---

## Quick Start

1. Check foundation chain requirements in CLAUDE.md (Vision, Strategy, Metrics, Opportunities, Capacity)
2. Choose narrative mode based on audience
3. Use Now-Next-Later format with appropriate confidence levels
4. See `## Roadmap` in `resources.md` for knowledge (Core first, Additional as needed)

---

## Co-Creation Flow (Default)

Build roadmap element by element with the user. This is the default mode.

### Flow Overview

```
Element 1: Narrative Mode    → Who's the audience and what story?
Element 2: Now Initiatives   → What's committed for this quarter?
Element 3: Next Initiatives  → What's planned for next quarter?
Element 4: Later Initiatives → What's directional for future?
Element 5: Trade-offs        → What's explicitly NOT on the roadmap?
Element 6: Sequencing        → Why this order?
→ [Assemble roadmap]
```

### Element-by-Element Process

**Element 1: Narrative Mode**
- Explain: "Narrative mode is how you tell the roadmap story. Different audiences need different framings: Vision-Driven (for team inspiration), KPI-Driven (for execs), Problem-Driven (for product teams), etc."
- Ask: "Who's the primary audience for this roadmap? What story do they need to hear?"
- Reflect back, confirm before continuing

**Element 2: Now Initiatives (Current Quarter)**
- Explain: "Now is high confidence, committed work. These are the initiatives you're actively building this quarter."
- Ask: "What initiatives are you committed to this quarter? What's actively being built?"
- For each initiative mentioned, ask: "What's the narrative framing? Why this, why now?"
- Reflect back, confirm before continuing

**Element 3: Next Initiatives (Following Quarter)**
- Explain: "Next is medium confidence, planned work. These are initiatives you intend to do but haven't committed to yet."
- Ask: "What's planned for next quarter? What do you intend to work on after Now?"
- For each initiative mentioned, ask: "What's the narrative framing?"
- Reflect back, confirm before continuing

**Element 4: Later Initiatives (Future)**
- Explain: "Later is low confidence, directional. These are things you're thinking about but aren't planning in detail."
- Ask: "What's on the horizon for the future? Directional themes, not commitments."
- Reflect back, confirm before continuing

**Element 5: Trade-offs**
- Explain: "Trade-offs are what's NOT on the roadmap. Being explicit about what you're not doing is as important as what you are doing."
- Ask: "What's explicitly NOT on this roadmap? What reasonable things are you choosing not to do?"
- Reflect back, confirm before continuing

**Element 6: Sequencing Rationale**
- Explain: "Sequencing rationale is the 'why this order' explanation. It connects the roadmap to strategy and makes the logic clear."
- Ask: "Why this sequence? What's the logic that drives Now before Next before Later?"
- Reflect back, confirm before continuing

### After All Elements

1. Summarize the roadmap (narrative mode, Now/Next/Later, trade-offs, sequencing)
2. Ask: "Anything to adjust before I assemble the roadmap?"
3. Assemble full roadmap document
4. Run verification checks
5. Save to `outputs/roadmap-[date].md`

### Skip Option

If user says "just draft it" or "skip ahead":
- Respect the request
- Draft based on available context
- Mark gaps with `[Needs input: ...]`

---

## Core Purpose

**Roadmap answers:**
- What are we building and when?
- Why are we building this (in this order)?
- How does this connect to our strategy?
- What story does this roadmap tell?

**Roadmap is NOT:**
- Strategy definition (see `strategy` skill)
- Problem validation (see `discovery` skill)
- Stakeholder coordination (see `stakeholder` skill)

---

## Key Responsibilities

1. **Initiative Planning** - Sequence initiatives based on strategy and validation
2. **Roadmap Storytelling** - Choose narrative mode for audience
3. **One-Pager Creation** - Document initiatives using Product Alignment Document
4. **Trade-off Communication** - Explain what's in vs out and why

---

## Core Concepts

- Now = high confidence, committed | Next = medium, planned | Later = low, directional
- Choose narrative mode for audience (Vision-Driven, KPI-Driven, Executive Pitch, etc.)

---

## Output Format

**Primary artifact:** Roadmap view (Now-Next-Later)

```
## NOW (Current Quarter)
[Initiative 1] - [Narrative framing]
[Initiative 2] - [Narrative framing]

## NEXT (Following Quarter)
[Initiative 3] - [Narrative framing]

## LATER (Future)
[Initiative 4] - [Narrative framing]
```

**Supporting artifacts:**
- Initiative one-pagers (Product Alignment Document)
- Roadmap narrative (chosen storytelling mode)

---

## Success Criteria

1. Roadmap tells a coherent story
2. Initiatives ladder up to strategy
3. Trade-offs are explicit and explained
4. Appropriate detail level per time horizon
5. Stakeholders understand the "why"

---

## Common Pitfalls

1. **Feature list masquerading as roadmap** - Include narrative, not just items
2. **Over-committing dates** - Use Now-Next-Later, protect flexibility
3. **Missing strategy connection** - Every initiative should ladder up
4. **Single narrative mode** - Adapt storytelling to audience
5. **Skipping one-pagers** - Document initiatives for alignment

---

## Verification Criteria

Before presenting roadmap deliverable, run these checks. Maximum 3 regeneration attempts per failed check.

### Foundation Prerequisites

**STOP if any of these are missing:**
- [ ] **Vision exists** - context/vision.md must exist
- [ ] **Strategy exists** - context/strategy.md must exist
- [ ] **Metrics defined** - Success metrics must be clear (from context/metrics.md or strategy)
- [ ] **Opportunities identified** - At least 1 validated opportunity exists (from context/opportunities.md or discovery work)
- [ ] **Capacity understood** - Team size or constraints mentioned (from context/company-profile.md or user input)

**If any missing:** Warn user and recommend building foundation first. User can override and proceed with gaps.

### Structural Requirements

**Core Components:**
- [ ] **Now-Next-Later structure** - Uses three time horizons
- [ ] **Now section populated** - At least 1 initiative in Now (current quarter)
- [ ] **Initiatives have narrative framing** - Each initiative includes "why" not just "what"
- [ ] **Saved to context** - Saved to `outputs/roadmap-[date].md`

### Quality Checks

**Strategic Alignment:**
- [ ] **Initiatives ladder to strategy** - Each Now initiative explicitly connects to strategic priorities
- [ ] **Supports metrics** - Clear how initiatives will move key metrics
- [ ] **Trade-offs explicit** - What's NOT on roadmap and why

**Capacity Realism:**
- [ ] **Acknowledges team size** - Roadmap considers capacity constraints (3 engineers ≠ 30 engineers)
- [ ] **Realistic scope** - Now items are achievable within timeframe given team size
- [ ] **Not over-committed** - Doesn't promise everything in Now

**Opportunity Connection:**
- [ ] **Based on validated opportunities** - Now initiatives come from discovery work, not random ideas
- [ ] **Addresses real problems** - Initiatives solve validated user problems

**Storytelling:**
- [ ] **Coherent narrative** - Roadmap tells a story (not just a list)
- [ ] **Narrative mode chosen** - Clear storytelling approach for audience (Vision-Driven, KPI-Driven, etc.)
- [ ] **Explains sequencing** - Clear why these initiatives in this order

**Confidence Levels:**
- [ ] **Now = High confidence** - Committed initiatives with clear scope
- [ ] **Next = Medium confidence** - Planned but flexible
- [ ] **Later = Low confidence** - Directional, not commitments

**Format Quality:**
- [ ] **Not a feature list** - Initiatives are outcome/opportunity-focused, not feature lists
- [ ] **Appropriate detail** - More detail in Now, less in Later
- [ ] **Avoids date commitments** - Uses time horizons, not specific dates (unless explicitly needed)

### Verification Process

1. **Check foundation prerequisites first** - If missing, warn and get user permission to proceed
2. Generate draft roadmap
3. Run all checks above
4. For each failed check:
   - **Can we fix with context we have?** → Regenerate silently
   - **Need user input?** → Ask specific question, then regenerate
5. Show progress: "Checking [criterion]... ✓ or ✗ [reason]"
6. Maximum 3 attempts per check
7. If still failing after 3 attempts → Proceed with warning: "⚠ Could not verify [criterion] after 3 attempts"
8. Present roadmap with Eval Summary appended

### Eval Summary Format

Append to roadmap deliverable:

```markdown
---
## Eval Summary

### Foundation Prerequisites
- [✓] Vision exists
- [✓] Strategy exists
- [✓] Metrics defined
- [✓] Opportunities identified (3 validated)
- [✓] Capacity understood

### Structural Requirements
- [✓] Now-Next-Later structure
- [✓] Now section populated (2 initiatives)
- [✓] Initiatives have narrative framing
- [✓] Saved to outputs

### Quality Checks - Strategic Alignment
- [✓] Initiatives ladder to strategy
- [✓] Supports metrics (activation rate, retention)
- [✓] Trade-offs explicit (not building X, Y because...)

### Quality Checks - Capacity Realism
- [✓] Acknowledges team size
- [✓] Realistic scope
- [✓] Not over-committed

### Quality Checks - Opportunity Connection
- [✓] Based on validated opportunities
- [✓] Addresses real problems

### Quality Checks - Storytelling
- [✓] Coherent narrative
- [✓] Narrative mode chosen (KPI-Driven for exec team)
- [✓] Explains sequencing

### Quality Checks - Confidence Levels
- [✓] Now = High confidence
- [✓] Next = Medium confidence
- [✓] Later = Low confidence

### Quality Checks - Format Quality
- [✓] Not a feature list
- [✓] Appropriate detail
- [✓] Avoids date commitments
```

Use:
- `[✓]` for passed checks
- `[✗]` for failed checks (with reason)
- `[ ]` for not applicable (with reason)
- `[⚠]` for foundation gaps (user proceeded anyway)
