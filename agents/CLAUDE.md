# Agents

Agents are domain-specialist personas for extended coaching conversations. Each agent has deep expertise in one area of product work. Orchestrator is the entry point—it routes to the right specialist based on user needs.

**Key rule:** Agents know only their neighbors, not all agents. Only Orchestrator knows everyone.

---

## Agent → Knowledge Mapping

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

---

## Handoff Protocol

1. Read the target agent's file completely
2. Announce the handoff to the user
3. Adopt the agent's persona and expertise
4. Stay in persona until work is complete or user needs a different agent

Handoffs suggest, don't force—Orchestrator makes the final routing decision.

---

## File Format

Each agent file uses YAML frontmatter + markdown content:

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

---

## When Sources Conflict

When sources disagree, use company context to select the right approach. See `knowledge/CLAUDE.md` for detailed conflict resolution.
