# Context

Foundational context about the company, user, and product.

## Files

| File | Purpose | Priority |
|------|---------|----------|
| `user-profile.md` | User role, experience → Sets conversation TONE | Built first (quick) |
| `company-profile.md` | Company stage, funding, business model | ESSENTIAL for PM work |
| `product-profile.md` | Product features, metrics, users | Built as needed |
| `sessions/` | Session summaries for multi-conversation memory | End of session |
| `uploads/` | User documents (pitch decks, strategy docs) | Optional input |

## How Context Gets Built

**Orchestrator handles context building automatically.** No manual setup required.

### First-Time Users (Empty Profiles)

When profiles are empty, Orchestrator:
1. **Asks about user first** — Role, experience level (sets tone)
2. **Offers company profile options:**
   - A) Upload files to `uploads/` → AI builds profile
   - B) Quick interview (5-6 questions)
   - C) Skip (learn passively during conversation)
3. **Then answers original question** with context

### Why Company Context is Essential

Product Management IS Business Management. Advice quality depends on knowing:
- Company stage (pre-PMF vs Series B = different PM work)
- Business model (B2B vs B2C = different approaches)
- Team size and structure
- Current focus and challenges

→ See `knowledge/alignment/product-management-is-business-management.md`

### Returning Users (Profiles Exist)

Orchestrator reads profiles and proceeds directly to their question.

## Rules

1. **User first, company second** — User context sets tone for company questions
2. **Never block user** — If they want to skip, let them
3. **Passive listening** — Pick up context clues during conversation
4. **Ask before saving** — "Can I add this to your profile?"
5. **Save sessions at end** — Offer to save summary for continuity

→ Full onboarding flow defined in `agents/orchestrator.md`
→ Session format in `sessions/CLAUDE.md`

## Profile Templates

Templates (`.template.md`) are tracked in git. Filled versions are gitignored.

Orchestrator creates profiles automatically through conversation. Manual creation not required.
