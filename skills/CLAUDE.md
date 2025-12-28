# Skills

All capabilities live here as `SKILL_NAME/SKILL.md` files with YAML frontmatter.

---

## Skill Hierarchy

```
ENTRY POINT
───────────────────────────────────────────────────────
using-productkit    →    (auto-injected at session start)

MAIN SKILLS              UTILITY SKILLS
───────────────────────────────────────────────────────
vision              →    (none)
    ↓
strategy            →    positioning
    ↓
    ├── discovery   →    opportunity-tree, interview-summary
    │
    └── metrics     →    okr-builder, metric-selector,
                         impact-model-builder, leading-lagging-mapper,
                         aarrr-analyzer
    ↓
roadmap             →    initiative-alignment-doc, prioritization
stakeholder         →    initiative-alignment-doc

EXECUTION WORKFLOW
───────────────────────────────────────────────────────
writing-pm-plans         →    (break down initiatives)
executing-pm-plans       →    (implement with checkpoints)
verification-before-completion → (verify before claiming done)

META
───────────────────────────────────────────────────────
skill-creator       →    (for building new skills)
```

**Foundation chain:** `Vision → Strategy → Metrics → Discovery → Roadmap`

**Notes:**
- STOP before Roadmap: must have metrics and opportunities first
- A roadmap without opportunities is just a feature list

---

## Stage Awareness (Strict)

When working through the foundation chain, users need to know where they are.

### Show Current Position

At each stage, state where user is:

"We're in **Strategy** (step 2 of 5 in the foundation chain)"

When helpful, show visual:
```
Vision ✓ → [Strategy] → Metrics → Discovery → Roadmap
            └─ you are here
```

### Explicit Handoffs

Never silently transition between main skills. Always:

1. **Summarize** what was completed: "We've defined your vision: [1-sentence summary]"
2. **State next step** and why: "This becomes the foundation for strategy."
3. **Ask permission**: "Ready to move to Strategy, or want to refine vision first?"

### Saving Context

Before transitioning to next skill:
1. Save work to `context/[skill].md` (e.g., `context/vision.md`)
2. If incomplete, use `[Needs input: ...]` placeholders and mark as draft
3. Offer one-pager: "Want a [Vision One-Pager] as a deliverable? (useful for stakeholder alignment)"

---

## Skill Index

| Skill | When to Use |
|-------|-------------|
| **ENTRY POINT** | |
| `using-productkit` | Session start, how ProductKit works, which skill to use |
| **MAIN SKILLS** | |
| `vision` | Vision, purpose, mission, long-term direction (3-5+ years) |
| `strategy` | Strategy, positioning, differentiation, "how to win" |
| `discovery` | Problem validation, user research, "is this worth building" |
| `metrics` | OKRs, KPIs, success measurement, leading indicators |
| `roadmap` | Roadmap, initiative planning, "what to build when" |
| `stakeholder` | Stakeholder alignment, getting buy-in, cross-team coordination |
| **UTILITY SKILLS** | |
| `positioning` | Positioning product, differentiation, crafting messaging |
| `opportunity-tree` | Structuring opportunities, building OST |
| `interview-summary` | Synthesizing interviews into snapshots |
| `okr-builder` | Setting OKRs, defining quarterly goals |
| `metric-selector` | Choosing KPIs, "what should we measure" |
| `impact-model-builder` | Building driver trees, connecting metrics to goals |
| `leading-lagging-mapper` | Indicator relationships, "what predicts outcomes" |
| `aarrr-analyzer` | Analyzing funnels, "where is funnel breaking" |
| `initiative-alignment-doc` | Documenting initiatives, alignment docs |
| `prioritization` | Comparing roadmap options, ranking features, "what should we focus on" |
| **EXECUTION WORKFLOW** | |
| `writing-pm-plans` | Breaking down PM initiatives, creating execution plans |
| `executing-pm-plans` | Implementing plans with checkpoints, resuming work |
| `verification-before-completion` | Verifying deliverables meet success criteria |
| **META** | |
| `skill-creator` | Building new skills, creating SKILL.md files |

---

## Tool Compatibility

**Claude Code:** Auto-discovers skills from YAML frontmatter. No manual loading needed.

**Cursor, Codex, Gemini CLI:** Read this index, then:
1. Match user intent to the right skill based on descriptions above
2. Load the relevant `SKILL_NAME/SKILL.md` file
3. Follow its instructions

---

## File Format

Each SKILL.md uses YAML frontmatter:

```yaml
---
name: skill-name
description: Use when [triggers only]. Never summarize workflow.
---
```

---

## Output Quality

Before finalizing any output, verify it follows `style-guide.md` structure:
1. **Overview** - 2-3 sentences: what, why now, what decision
2. **Main content** - Document-specific sections
3. **FAQ** - Strategic questions with `[Suggested answer - Please review]` prefix
