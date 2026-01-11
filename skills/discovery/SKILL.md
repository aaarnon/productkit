---
name: discovery
description: Use when discussing problem validation, user research, opportunity mapping, assumptions testing, or "is this worth building."
---

# Discovery

Validates problems and maps opportunities before committing to solutions. Focuses on understanding user needs, validating assumptions, and building the opportunity backlog.

---

## Quick Start

1. Frame the opportunity as a capability (what users can achieve), not a feature
2. Assess four risks: Value, Usability, Feasibility, Business Viability
3. Determine confidence level needed for decision
4. Recommend: Backlog, Parking Lot, or Bin

---

## Co-Creation Flow (Default)

Build validated opportunity element by element with the user. This is the default mode.

### Flow Overview

```
Section 1: Opportunity Framing (2 elements)
  → Opportunity Statement → Problem Evidence
  → [Confirm section before continuing]

Section 2: Risk Assessment (4 elements)
  → Value Risk → Usability Risk → Feasibility Risk → Business Viability Risk
  → [Confirm section before continuing]

Section 3: Decision (2 elements)
  → Confidence Level → Recommendation
  → [Assemble validated opportunity]
```

### Section 1: Opportunity Framing

**Element 1: Opportunity Statement**
- Explain: "The opportunity statement describes what users will be able to achieve. Frame it as a capability, not a feature."
- Ask: "What will users be able to do or achieve? (Not 'add a dashboard' but 'users can track their progress at a glance.')"
- Reflect back, confirm before continuing

**Element 2: Problem Evidence**
- Explain: "Problem evidence is the research, data, or feedback that supports this opportunity. What makes you believe this is real?"
- Ask: "What evidence do you have that this is a real problem worth solving? User interviews, data, support tickets, etc."
- Reflect back, confirm before continuing

**Section Checkpoint:**
- Summarize the opportunity framing
- Ask: "Anything to adjust before we assess the risks?"

### Section 2: Risk Assessment

**Element 3: Value Risk**
- Explain: "Value risk is whether users actually want this. Will they care enough to use it?"
- Ask: "How confident are you that users actually want this? What evidence supports or contradicts that? (Low/Medium/High risk)"
- Reflect back, confirm before continuing

**Element 4: Usability Risk**
- Explain: "Usability risk is whether users can figure out how to use it. Will they understand it?"
- Ask: "How confident are you that users will understand how to use this? Any complexity concerns? (Low/Medium/High risk)"
- Reflect back, confirm before continuing

**Element 5: Feasibility Risk**
- Explain: "Feasibility risk is whether you can actually build it. Technical constraints, dependencies, unknowns."
- Ask: "How confident are you that you can build this? Any technical challenges or unknowns? (Low/Medium/High risk)"
- Reflect back, confirm before continuing

**Element 6: Business Viability Risk**
- Explain: "Business viability risk is whether this makes sense for the business. Alignment with strategy, revenue impact, resource cost."
- Ask: "How confident are you this is good for the business? Does it align with strategy and justify the investment? (Low/Medium/High risk)"
- Reflect back, confirm before continuing

**Section Checkpoint:**
- Summarize all four risks
- Ask: "Anything to adjust before we determine confidence and recommendation?"

### Section 3: Decision

**Element 7: Confidence Level**
- Explain: "Confidence level is your overall certainty about this opportunity. Based on evidence quality and risk levels."
- Ask: "Given everything we've discussed, how confident are you overall? (Low/Medium/High) Why?"
- Reflect back, confirm before continuing

**Element 8: Recommendation**
- Explain: "Recommendation is the action: Backlog (build it), Parking Lot (needs more validation), or Bin (don't pursue)."
- Ask: "Based on confidence and risks, what's the recommendation? Backlog, Parking Lot, or Bin?"
- Reflect back, confirm before continuing

### After All Elements

1. Summarize the validated opportunity (statement, evidence, risks, confidence, recommendation)
2. Ask: "Anything to adjust before I assemble the opportunity document?"
3. Assemble full validated opportunity
4. Run verification checks
5. Save to `context/opportunities.md`

### Skip Option

If user says "just draft it" or "skip ahead":
- Respect the request
- Draft based on available context
- Mark gaps with `[Needs input: ...]`

---

## Core Purpose

**Discovery answers:**
- What problems are worth solving?
- How do we know this is the right problem?
- What opportunities exist?
- How confident are we in our assumptions?

**Discovery is NOT:**
- Solution definition (that comes after validation)
- Roadmap planning (see `roadmap` skill)
- Execution planning

---

## Key Responsibilities

1. **Problem Validation** - Validate that problems are real and worth solving
2. **Opportunity Mapping** - Create and prioritize opportunity trees
3. **Risk Assessment** - Evaluate Value, Usability, Feasibility, Business Viability risks
4. **Confidence Building** - Gather evidence through research and validation
5. **Interview Synthesis** - Transform customer conversations into actionable insights

---

## Core Concepts

- Four Risks: Value, Usability, Feasibility, Business Viability
- Frame as capabilities (what users achieve), not features
- Triage to: Backlog, Parking Lot, or Bin

---

## Output Format

**Primary artifact:** Validated opportunity

```
## Opportunity Statement
[Capability framing - what users will be able to achieve]

## Problem Evidence
[Research, data, feedback supporting this]

## Risk Assessment
- Value: [Low/Medium/High] - [Evidence]
- Usability: [Low/Medium/High] - [Evidence]
- Feasibility: [Low/Medium/High] - [Evidence]
- Business Viability: [Low/Medium/High] - [Evidence]

## Confidence Level
[Low/Medium/High] - [Justification]

## Recommendation
[Backlog / Parking Lot / Bin]
```

---

## Success Criteria

1. Problems validated with evidence (not assumptions)
2. Opportunities framed as capabilities (not features)
3. Risks explicitly assessed
4. Appropriate confidence level for decision
5. Clear recommendation (build, defer, or kill)

---

## Common Pitfalls

1. **Solution-first thinking** - Start with problem, not solution
2. **Over-researching** - Know when enough evidence is enough
3. **Feature framing** - Frame as capabilities, not features
4. **Skipping risk assessment** - Always assess all four risks
5. **Assumption validation theater** - Seek disconfirming evidence too

---

## Verification Criteria

Before presenting discovery deliverable, run these checks. Maximum 3 regeneration attempts per failed check.

### Foundation Prerequisites

**Check before creating discovery deliverable:**
- [ ] **Vision exists** - context/vision.md must exist
- [ ] **Strategy exists** - context/strategy.md must exist

**If missing:** Warn user and recommend building foundation first. User can override and proceed with gaps.

### Structural Requirements

**Core Components:**
- [ ] **Opportunity Statement exists** - Clear statement of the capability or opportunity
- [ ] **Problem Evidence provided** - Research, data, or feedback supporting this
- [ ] **Risk Assessment complete** - All four risks assessed (Value, Usability, Feasibility, Business Viability)
- [ ] **Confidence Level stated** - Low/Medium/High with justification
- [ ] **Recommendation clear** - Backlog, Parking Lot, or Bin decision stated
- [ ] **Saved to context** - Saved to `context/opportunities.md` or appropriate location

### Quality Checks

**Strategic Alignment:**
- [ ] **Connected to strategy** - Opportunity aligns with strategic priorities in context/strategy.md
- [ ] **Supports metrics** - Opportunity would move key metrics if successful
- [ ] **Worth solving** - Problem is significant enough to warrant investment

**Problem Validation:**
- [ ] **Evidence-backed** - Claims supported by research, data, or user feedback (not just assumptions)
- [ ] **Specific problem** - Problem is concrete, not vague ("users are confused by X" not "experience could be better")
- [ ] **Target user identified** - Clear who experiences this problem
- [ ] **Disconfirming evidence sought** - Attempted to invalidate, not just confirm

**Opportunity Framing:**
- [ ] **Framed as capability** - Describes what users will achieve, not features to build ("Users can track progress" not "Add a dashboard")
- [ ] **Outcome-focused** - Focuses on user outcome, not solution
- [ ] **Actionable** - Clear enough to guide solution exploration

**Risk Assessment:**
- [ ] **All four risks assessed** - Value, Usability, Feasibility, Business Viability all evaluated
- [ ] **Risk levels justified** - Each risk has supporting evidence or reasoning
- [ ] **Risks are honest** - Not sugar-coated or overly optimistic
- [ ] **High risks acknowledged** - If any risk is High, it's explicitly addressed in recommendation

**Confidence and Recommendation:**
- [ ] **Confidence justified** - Level matches amount and quality of evidence
- [ ] **Recommendation matches confidence** - High confidence + low risk = Backlog; Low confidence or high risk = Parking Lot or Bin
- [ ] **Next steps clear** - If Parking Lot, states what's needed to move forward

### Verification Process

1. Generate draft validated opportunity
2. Run all checks above
3. For each failed check:
   - **Can we fix with context we have?** → Regenerate silently
   - **Need user input?** → Ask specific question, then regenerate
4. Show progress: "Checking [criterion]... ✓ or ✗ [reason]"
5. Maximum 3 attempts per check
6. If still failing after 3 attempts → Proceed with warning: "⚠ Could not verify [criterion] after 3 attempts"
7. Present opportunity with Eval Summary appended

### Eval Summary Format

Append to discovery deliverable:

```markdown
---
## Eval Summary

### Foundation Prerequisites
- [✓] Vision exists
- [✓] Strategy exists

### Structural Requirements
- [✓] Opportunity Statement exists
- [✓] Problem Evidence provided
- [✓] Risk Assessment complete (all 4 risks)
- [✓] Confidence Level stated (Medium)
- [✓] Recommendation clear (Backlog)
- [✓] Saved to context

### Quality Checks - Strategic Alignment
- [✓] Connected to strategy
- [✓] Supports metrics
- [✓] Worth solving

### Quality Checks - Problem Validation
- [✓] Evidence-backed (5 user interviews)
- [✓] Specific problem
- [✓] Target user identified
- [✓] Disconfirming evidence sought

### Quality Checks - Opportunity Framing
- [✓] Framed as capability
- [✓] Outcome-focused
- [✓] Actionable

### Quality Checks - Risk Assessment
- [✓] All four risks assessed
- [✓] Risk levels justified
- [✓] Risks are honest
- [✓] High risks acknowledged (Feasibility: High due to tech constraints)

### Quality Checks - Confidence and Recommendation
- [✓] Confidence justified (Medium - validated problem, uncertain solution)
- [✓] Recommendation matches confidence
- [✓] Next steps clear (prototype needed to validate usability)
```

Use:
- `[✓]` for passed checks
- `[✗]` for failed checks (with reason)
- `[ ]` for not applicable (with reason)
