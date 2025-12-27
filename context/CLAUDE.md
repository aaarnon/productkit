# Context

Context files store foundational information about the company, user, product, and strategic direction. This is what makes ProductKit's advice relevant—generic PM advice is useless without knowing the company's stage, business model, and challenges.

**Product Management IS Business Management.** Advice quality depends entirely on context.

---

## Files

### Profiles

| File | Purpose | When Built |
|------|---------|------------|
| `user-profile.md` | Role, experience → Sets conversation tone | First (quick) |
| `company-profile.md` | Stage, funding, business model | Essential for PM work |
| `product-profile.md` | Current state: metrics, features, friction (not strategy) | As needed |

### Strategic Foundation (Cascade)

These files form a dependency chain. Each layer requires the one above.

```
vision.md → strategy.md → roadmap.md
```

| File | Purpose | Requires | Enables |
|------|---------|----------|---------|
| `vision.md` | Why we exist, where we're going (3-5+ years) | — | Strategy work |
| `strategy.md` | How we win (Narrative, Playing Field, Winning Moves) | vision.md | Roadmap work |
| `roadmap.md` | What we're building, in what order (point-in-time, dated) | vision.md, strategy.md | Prioritization, OKRs |

**Why this matters:** Skipping foundations creates weak outputs. A roadmap without strategy is just a feature list. Strategy without vision is tactics without direction.

### Multi-Product Companies

Default structure assumes single product. For multi-product companies:

```
context/
├── company-profile.md         # Shared
├── user-profile.md            # Shared
├── vision.md                  # Company-level vision (optional)
├── products/
│   ├── [product-a]/
│   │   ├── profile.md
│   │   ├── vision.md
│   │   ├── strategy.md
│   │   └── roadmap.md
│   └── [product-b]/
│       └── ...
```

When `products/` folder exists, orchestrator asks "Which product?" before routing.

### Other

| File | Purpose |
|------|---------|
| `sessions/` | Session summaries for memory |
| `uploads/` | User documents (pitch decks, etc.) |
| `templates/` | All templates (.template.md files) |

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

Templates live in `templates/` folder and are tracked in git. Filled versions (in root context/) are gitignored.

| Template | Creates |
|----------|---------|
| `templates/user-profile.template.md` | `user-profile.md` |
| `templates/company-profile.template.md` | `company-profile.md` |
| `templates/product-profile.template.md` | `product-profile.md` |
| `templates/vision.template.md` | `vision.md` |
| `templates/strategy.template.md` | `strategy.md` |
| `templates/roadmap.template.md` | `roadmap.md` |

Orchestrator creates these through conversation. Manual creation not required.

→ Full onboarding flow in `.claude/skills/orchestrator/SKILL.md`
→ Session format in `sessions/CLAUDE.md`
