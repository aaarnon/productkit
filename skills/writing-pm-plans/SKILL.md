---
name: writing-pm-plans
description: Use when breaking down PM initiatives into tasks, planning complex product work, or creating execution plans before starting work.
---

# Writing PM Plans

## Overview

Write comprehensive execution plans for PM initiatives. Plans assume the executor may return days later with limited context.

**Announce at start:** "Using writing-pm-plans to create the execution plan."

**Save plans to:** `outputs/plans/YYYY-MM-DD-[initiative-name].md`

---

## When to Use

- Initiative spans multiple deliverables
- Cross-functional coordination needed
- Work will span multiple sessions
- Complex stakeholder alignment required

---

## Plan Document Header

Every plan MUST start with:

```markdown
# [Initiative Name] Execution Plan

> **For Claude:** Use productkit:executing-pm-plans to implement this plan.

**Goal:** [One sentence - what this produces]

**Success Criteria:** [How we know it's done]

**Red/Blue Mode:** [Execution/Discovery] - [Why]

**Foundation Status:**
- Vision: [Exists/Missing]
- Strategy: [Exists/Missing]
- Roadmap: [Exists/Missing]

---
```

---

## Task Granularity

Each task = one focused work session (30-60 min equivalent).

**Good task:**
- "Draft problem definition section of alignment doc"
- "Synthesize 3 customer interviews into opportunity tree"
- "Create prioritized initiative list using VEUC framework"

**Bad task (too big):**
- "Create full product strategy"
- "Do discovery research"
- "Build complete roadmap"

**Bad task (too small):**
- "Write one bullet point"
- "Add header to document"
- "Fix typo"

---

## Task Structure

```markdown
### Task N: [Task Name]

**Deliverable:** [What gets created/updated]

**Location:** `outputs/[filename]` or `context/[filename]`

**Inputs needed:**
- [Existing context files]
- [Information to gather]

**Steps:**
1. [Specific action]
2. [Specific action]
3. [Verification step]

**Success criteria:**
- [ ] [Measurable outcome 1]
- [ ] [Measurable outcome 2]

**Checkpoint:** [When to pause for review]
```

---

## PM-Specific Checkpoints

Unlike code (commit after each task), PM work uses strategic checkpoints:

| After... | Checkpoint |
|----------|------------|
| Foundation work (vision/strategy) | Review before building on it |
| Problem definition | Validate before solution design |
| Draft deliverable | Review before finalizing |
| Cross-functional impact | Stakeholder alignment |

---

## Example Plan Skeleton

```markdown
# Q1 Roadmap Creation Plan

> **For Claude:** Use productkit:executing-pm-plans to implement.

**Goal:** Create Q1 roadmap with initiative one-pagers

**Success Criteria:**
- Roadmap in Now-Next-Later format
- Top 3 initiatives have alignment docs
- Stakeholder review scheduled

**Red/Blue Mode:** Red (Execution) - PMF established, optimizing

**Foundation Status:**
- Vision: Exists (context/vision.md)
- Strategy: Exists (context/strategy.md)
- Roadmap: Creating

---

### Task 1: Audit Current State

**Deliverable:** Gap analysis (conversation, not saved)

**Steps:**
1. Read context/strategy.md for strategic priorities
2. List initiatives already in progress
3. Identify gaps between strategy and current work

**Success criteria:**
- [ ] Strategic themes identified
- [ ] In-progress initiatives listed
- [ ] Gaps articulated

**Checkpoint:** Review gaps before prioritization

---

### Task 2: Prioritize Initiative Candidates

**Deliverable:** Prioritized initiative list
**Location:** outputs/q1-initiatives-draft.md

**Steps:**
1. Invoke prioritization skill
2. Apply VEUC or DHM framework
3. Create ranked list with rationale

**Success criteria:**
- [ ] 5-7 candidate initiatives
- [ ] Clear prioritization rationale
- [ ] Trade-offs documented

**Checkpoint:** Stakeholder input on priorities

---

[Continue with tasks 3-N...]
```

---

## Execution Handoff

After saving the plan:

"Plan saved to `outputs/plans/[filename].md`. Ready to execute?

**Options:**
1. **Continue now** - Use executing-pm-plans skill
2. **Pause for review** - Review plan first, execute later
3. **Share plan** - Get stakeholder input before executing

Which approach?"

---

## Remember

- Task = one session of focused work
- Include success criteria for every task
- Specify checkpoint moments
- Reference other skills when needed (prioritization, metrics, etc.)
- Use `[Needs input: ...]` for information gaps
