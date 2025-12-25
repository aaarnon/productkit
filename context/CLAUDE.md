# Context

Foundational context about the company, user, and product. **Check before any agent routing.**

## Files

| File | Purpose |
|------|---------|
| `company-profile.md` | Company stage, funding, team, business model |
| `user-profile.md` | User role, experience, preferences |
| `product-profile.md` | Product features, metrics, users, roadmap |
| `sessions/` | Session summaries for multi-conversation memory |
| `uploads/` | User documents (pitch decks, strategy docs) |

## Rules

1. **Check profiles first** — Before routing to any agent
2. **Never block user** — If they want to skip context, let them
3. **Passive listening** — Pick up context clues during conversation
4. **Suggest updates, don't auto-update** — Ask before saving to profiles
5. **Save sessions at end** — Offer to save summary for continuity

→ See `sessions/CLAUDE.md` for session format.
→ Context building behavior is defined in `agents/orchestrator.md`.

## Profile Templates

Templates are provided as `.template.md` files (tracked in git). The filled versions are gitignored.

**First-time setup:**
```bash
cp company-profile.template.md company-profile.md
cp user-profile.template.md user-profile.md
cp product-profile.template.md product-profile.md
```

Then fill through conversation or direct editing.
