# Skills

Skills are discrete tools that produce specific outputs. Unlike agents (extended conversations), skills run once and return a result—a prioritized list, an OKR draft, an opportunity tree, etc.

Skills can be invoked by users directly or called by agents during coaching sessions.

---

## Skill → Knowledge Mapping

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

---

## Invocation Modes

| Mode | Meaning | Example |
|------|---------|---------|
| **Hybrid** | User or agent can invoke | "Help me prioritize" triggers prioritization skill |
| **Agent-called** | Only agents invoke | OKR builder called by Metrics agent |

---

## File Format

Each skill file uses YAML frontmatter + markdown content:

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
