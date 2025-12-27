# Skills

All capabilities live here as `SKILL_NAME/SKILL.md` files with YAML frontmatter.

---

## Skill Types

### Conversation Modes
Extended guidance for multi-turn discussions. These help think through problems.

| Skill | Purpose |
|-------|---------|
| `orchestrator` | Routes to the right skill, coordinates across domains. Use when starting fresh or unsure where to begin. |
| `discovery` | Validates problems and maps opportunities. Use for problem validation, user research, assumption testing. |
| `strategy` | Defines how to win. Use for positioning, differentiation, competitive advantage. |
| `metrics` | Defines success measurement. Use for OKRs, KPIs, leading indicators, impact models. |
| `roadmap` | Plans and communicates initiatives. Use for sequencing, Now-Next-Later, roadmap artifacts. |
| `stakeholder` | Facilitates alignment and buy-in. Use for cross-functional coordination, RACI, getting people on board. |
| `vision` | Defines long-term purpose (3-5+ years). Use for mission, purpose, "why does this exist." |

### Output Tools
Discrete deliverables. These produce specific artifacts.

| Skill | Purpose |
|-------|---------|
| `prioritization` | Applies prioritization frameworks (VEUC, DHM). Outputs ranked options. |
| `okr-builder` | Creates Objectives and Key Results. Outputs OKR draft. |
| `opportunity-tree` | Creates Opportunity Solution Trees. Outputs prioritized OST. |
| `interview-summary` | Synthesizes customer interviews. Outputs one-page summary. |
| `positioning` | Creates positioning statements (April Dunford framework). Outputs positioning doc. |
| `metric-selector` | Selects success metrics (5-lenses). Outputs recommended metrics. |
| `impact-model-builder` | Creates driver trees. Outputs impact model. |
| `leading-lagging-mapper` | Maps indicator relationships. Outputs indicator chain. |
| `aarrr-analyzer` | Analyzes pirate funnel. Outputs funnel diagnosis. |
| `initiative-alignment-doc` | Creates alignment documents. Outputs initiative doc. |

---

## For Tools Without Auto-Discovery

If using Cursor or other tools that don't auto-discover skills:

1. Read this index to understand available skills
2. Match user intent to the right skill based on descriptions above
3. Load the relevant `SKILL_NAME/SKILL.md` file
4. Follow its instructions

---

## File Format

Each SKILL.md uses YAML frontmatter:

```yaml
---
name: skill-name
description: What it does + when to use it. Include trigger terms.
---
```

---

## Output Quality

Before finalizing any output, verify it follows `style-guide.md` structure:
1. **Overview** - 2-3 sentences: what, why now, what decision
2. **Main content** - Document-specific sections
3. **FAQ** - Strategic questions with `[Suggested answer - Please review]` prefix
