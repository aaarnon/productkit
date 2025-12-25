# Skills

## Format

Each skill file: YAML frontmatter + markdown content.

```yaml
---
name: skill-name
description: What it does + when to use it. Third person. Include trigger terms.
---
```

**Required sections:**
- Purpose (one line)
- Invocation (hybrid or agent-called)
- When to Use (trigger scenarios)
- Process/Template
- Output Format

→ Use `skill-creator.md` as reference when creating new skills.

## Skill → Folder Mapping

| Skill | Primary Knowledge Folder |
|-------|--------------------------|
| prioritization | `knowledge/prioritization/` |
| positioning | `knowledge/strategy/` |
| opportunity-tree | `knowledge/discovery/` |
| okr-builder | `knowledge/metrics/` |
| impact-model-builder | `knowledge/metrics/` |
| metric-selector | `knowledge/metrics/` |
| leading-lagging-mapper | `knowledge/metrics/` |
| aarrr-analyzer | `knowledge/metrics/` |
| initiative-alignment-doc | `knowledge/alignment/` |
| interview-summary | `knowledge/discovery/` |

→ See `knowledge/CLAUDE.md` for folder-based discovery and conflict handling.

## Invocation Modes

| Mode | Meaning |
|------|---------|
| **Hybrid** | User or agent can invoke |
| **Agent-called** | Only agents invoke |

**Current:** 11 skills (1 meta, 2 hybrid, 8 agent-called)
