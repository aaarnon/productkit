---
name: vision
description: Use when discussing vision, purpose, mission, long-term direction, or "why does this exist." (3-5+ year horizon)
---

# Vision

Defines the long-term purpose and direction of the product or business. Focuses on the "why" and aspirational future state (3-5+ year horizon).

---

## Quick Start

1. Answer: Why does this product/business exist?
2. Paint the 3-5 year aspirational future state
3. Test: Is it inspiring, clear, differentiating, and stable?
4. See `## Vision` in `resources.md` for knowledge (Core first, Additional as needed)
5. Save to `context/vision.md` (foundation for strategy)

---

## Co-Creation Flow (Default)

Build vision element by element with the user. This is the default mode.

### Flow Overview

```
Element 1: Purpose      → Why does this exist?
Element 2: Future State → Where do we want to be in 3-5 years?
Element 3: Impact       → What change do we want to make?
→ [Assemble vision statement]
```

### Element-by-Element Process

**Element 1: Purpose**
- Explain: "Purpose is why this product/business exists. Not what it does, but why it matters."
- Ask: "Why does [product/company] exist? What problem or need drives it?"
- Reflect back, confirm before continuing

**Element 2: Future State**
- Explain: "Future state is where you want to be in 3-5 years if everything goes right. Paint the picture."
- Ask: "If everything goes well, what does the world look like in 3-5 years because of [product/company]?"
- Reflect back, confirm before continuing

**Element 3: Impact**
- Explain: "Impact is the change you want to make. Who benefits and how?"
- Ask: "What lasting change do you want to create? Who's better off and in what way?"
- Reflect back, confirm before continuing

### After All Elements

1. Summarize what was captured across all three elements
2. Ask: "Anything to adjust before I draft the vision statement?"
3. Draft vision (1-2 paragraphs weaving purpose, future state, and impact)
4. Run verification checks
5. Save to `context/vision.md`

### Skip Option

If user says "just draft it" or "skip ahead":
- Respect the request
- Draft based on available context
- Mark gaps with `[Needs input: ...]`

---

## Core Purpose

**Vision answers:**
- Why does this product/business exist?
- What is the purpose we're serving?
- Where do we want to be in 3-5 years if everything goes right?
- What impact do we want to have?

**Vision is NOT:**
- Strategy (see `strategy` skill)
- Roadmap (see `roadmap` skill)
- Short-term goals (quarterly/annual)

---

## Key Responsibilities

1. **Define Purpose** - Articulate why the product/business exists
2. **Aspirational Future State** - Paint picture of success 3-5+ years out
3. **Vision Validation** - Test if vision is inspiring, clear, and differentiated
4. **Vision Communication** - Craft compelling narrative for stakeholders

---

## Core Concepts

- Validation tests: Inspiring, Clear, Differentiating, Actionable, Stable
- Vision = destination (3-5+ years), Strategy = path to get there

---

## Output Format

**Primary artifact:** Vision statement (1-2 paragraphs)

**Supporting artifacts:**
- Vision narrative (extended storytelling version)
- Vision rationale (evidence, market context)

---

## Success Criteria

1. Vision is inspiring and motivating
2. Vision provides clear direction
3. Vision is differentiated from competitors
4. Strategy can derive from vision
5. Vision is stable (not changing quarterly)

---

## Common Pitfalls

1. **Too tactical** - Vision should not be a feature list
2. **Too vague** - "Change the world" without specificity
3. **Too short-term** - Vision should be 3-5+ years, not 1 year
4. **Conflated with strategy** - Vision is destination, strategy is path
5. **Not inspiring** - Dry corporate-speak that doesn't motivate

---

## Verification Criteria

Before presenting vision deliverable, run these checks. Maximum 3 regeneration attempts per failed check.

**Structural Requirements:**
- [ ] **Purpose clarity** - Explicitly states why the product/business exists
- [ ] **Future state** - Describes aspirational state 3-5+ years out
- [ ] **Appropriate length** - 1-3 paragraphs (not single sentence, not essay)
- [ ] **No tactical content** - No features, roadmap items, or short-term goals mentioned
- [ ] **Saved to context** - Saved to `context/vision.md`

**Quality Checks:**
- [ ] **Clarity** - Specific enough to guide decisions, not generic platitudes
- [ ] **Differentiation** - Mentions specific impact or angle (not "be the best")
- [ ] **Inspiring tone** - Uses aspirational language, not dry corporate-speak
- [ ] **Time horizon** - References or implies 3-5+ year timeframe

**Verification Process:**

1. Generate draft vision statement
2. Run all checks above
3. For each failed check:
   - **Can we fix with context we have?** → Regenerate silently
   - **Need user input?** → Ask specific question, then regenerate
4. Show progress: "Checking [criterion]... ✓ or ✗ [reason]"
5. Maximum 3 attempts per check
6. If still failing after 3 attempts → Proceed with warning: "⚠ Could not verify [criterion] after 3 attempts"
7. Present vision with Eval Summary appended

**Eval Summary Format:**

Append to `context/vision.md` and any vision deliverable:

```markdown
---
## Eval Summary
- [✓] Purpose clarity verified
- [✓] Future state described
- [✓] Appropriate length
- [✓] No tactical content
- [✓] Saved to context
- [✓] Clarity verified
- [✓] Differentiation present
- [✓] Inspiring tone
- [✗] Time horizon - Could not verify after 3 attempts
```

Use:
- `[✓]` for passed checks
- `[✗]` for failed checks (with reason)
- `[ ]` for not applicable (with reason)
