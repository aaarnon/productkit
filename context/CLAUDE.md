# Context

Context files store foundational information about the company, user, and product. This is what makes PM-Copilot's advice relevant—generic PM advice is useless without knowing the company's stage, business model, and challenges.

**Product Management IS Business Management.** Advice quality depends entirely on context.

---

## Files

| File | Purpose | When Built |
|------|---------|------------|
| `user-profile.md` | Role, experience → Sets conversation tone | First (quick) |
| `company-profile.md` | Stage, funding, business model | Essential for PM work |
| `product-profile.md` | Features, metrics, users | As needed |
| `sessions/` | Session summaries for memory | End of session |
| `uploads/` | User documents (pitch decks, etc.) | Optional input |

---

## How Context Gets Built

**Orchestrator handles this automatically.** No manual setup required.

### First-Time Users (Empty Profiles)

1. **Ask about user first** — Role, experience level (sets tone)
2. **Offer company profile options:**
   - A) Upload files to `uploads/` → AI builds profile
   - B) Quick interview (5-6 questions)
   - C) Skip (learn passively during conversation)
3. **Then answer original question** with context

### Returning Users (Profiles Exist)

Read profiles and proceed directly to their question.

---

## Rules

- **User first, company second** — User context sets tone for company questions
- **Never block user** — If they want to skip, let them
- **Passive listening** — Pick up context clues during conversation
- **Ask before saving** — "Can I add this to your profile?"

---

## Learnings (Meta-Memory)

Profiles have a "Learnings" section for meta-patterns discovered over time.

**What to capture:**

| Profile | Examples |
|---------|----------|
| Company | "Struggles with prioritization", "Stakeholder buy-in is bottleneck" |
| User | "Prefers direct feedback", "Jumps to solutions before defining problems" |

**When to capture:**
- At checkpoints (before saving)
- When an approach fails ("We tried X, didn't work because Y")
- When you notice a recurring pattern

Don't interrupt conversation flow. Add at natural pauses.

---

## Checkpoint Saves

Users often close chat without warning. Save incrementally, not just at end.

| Trigger | Example Prompt |
|---------|----------------|
| After delivering artifact | "Created the roadmap. Save session? (helps me remember context)" |
| After significant decision | "We decided to focus on activation. Save this?" |
| After failed approach | "That framework didn't fit. Noting this." |
| Before topic switch | "Before we switch to metrics—save strategy context?" |

**Always explain why** — Users say yes more often when they understand the benefit.

---

## Templates

Templates (`.template.md`) are tracked in git. Filled versions are gitignored.

Orchestrator creates profiles through conversation. Manual creation not required.

→ Full onboarding flow in `agents/orchestrator.md`
→ Session format in `sessions/CLAUDE.md`
