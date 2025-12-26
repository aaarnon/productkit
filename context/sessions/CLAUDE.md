# Sessions

Session files enable multi-conversation memory. Claude reads recent sessions at conversation start to remember previous context, decisions, and open questions.

---

## File Naming

```
YYYY-MM-DD-[topic].md
```

Examples:
- `2025-12-25-roadmap-planning.md`
- `2025-12-28-metrics-review.md`

---

## Session Format

```markdown
# Session: [Topic]

**Date:** YYYY-MM-DD
**Primary Agent:** [Which agent was mostly used]

## Context
[What the user was trying to accomplish]

## Key Decisions
- [Decision 1]
- [Decision 2]

## Learnings About Company/Product
- [New info that should inform future sessions]

## Artifacts Created
- [Outputs: one-pagers, OKRs, roadmaps, etc.]

## Open Questions
- [Unresolved items for future sessions]

## Next Steps
- [What user planned to do next]
```

---

## Orchestrator Behavior

**Start of session:**
1. Check for recent session files (last 3-5)
2. Read them to rebuild context
3. Reference relevant history: "Last time we discussed X..."

**End of session:**
1. Offer to save session summary
2. If user agrees, create session file with descriptive topic name

---

## Retention

Keep sessions indefinitely. Archive old ones to `sessions/archive/` if folder gets large.
