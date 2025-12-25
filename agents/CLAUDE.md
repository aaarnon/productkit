# Agents

## Format

Each agent file: YAML frontmatter + markdown content.

```yaml
---
name: agent-name
description: What it does + when to use it. Include trigger terms.
---
```

**Required sections:**
- Role (1-2 sentences)
- Core Purpose (what it answers, what it's NOT)
- Key Responsibilities (3-5 items)
- Related Agents (neighbors + handoff triggers)
- Key Frameworks (summaries only)
- Output Format
- Common Pitfalls

## Agent → Folder Mapping

| Agent | Primary Knowledge Folders |
|-------|---------------------------|
| Orchestrator | `alignment/`, `prioritization/` |
| Vision | `strategy/`, `alignment/` |
| Strategy | `strategy/`, `prioritization/` |
| Discovery | `discovery/` |
| Roadmap | `roadmap/`, `alignment/` |
| Metrics | `metrics/` |
| Stakeholder | `alignment/` |

→ See `knowledge/CLAUDE.md` for folder-based discovery and conflict handling.

## Rules

- Agents know only their neighbors, not all agents
- Orchestrator is the only agent that knows all others
- Handoffs suggest, don't force — Orchestrator decides
- When sources conflict, use company context to select approach
