# Sessions

Auto-saved summaries from each conversation session.

## Purpose

Enables multi-session persistence - Claude remembers previous conversations by reading recent session summaries.

## File Naming

```
YYYY-MM-DD-[topic].md
```

Examples:
- `2025-12-25-roadmap-planning.md`
- `2025-12-28-metrics-review.md`
- `2025-01-05-discovery-interviews.md`

## Session Summary Format

Each session file should capture:

```markdown
# Session: [Topic]

**Date:** YYYY-MM-DD
**Duration:** ~X minutes
**Primary Agent:** [Which agent was mostly used]

## Context
[What the user was trying to accomplish]

## Key Decisions
- [Decision 1]
- [Decision 2]

## Learnings About Company/Product
- [New info learned that should inform future sessions]

## Artifacts Created
- [Any outputs: one-pagers, OKRs, roadmaps, etc.]

## Open Questions
- [Unresolved items for future sessions]

## Next Steps Discussed
- [What user planned to do next]
```

## Orchestrator Behavior

**Start of session:**
1. Check for recent session files (last 3-5)
2. Read them to rebuild context
3. Reference relevant history: "Last time we discussed X..."

**End of session:**
1. Offer to save session summary
2. If user agrees, create session file
3. Use descriptive topic name

## Retention

Keep sessions indefinitely or archive old ones to `sessions/archive/` if folder gets large.
