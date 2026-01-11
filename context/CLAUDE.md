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
context/vision.md → context/strategy.md → context/roadmap.md
```

| File | Purpose | Requires | Enables |
|------|---------|----------|---------|
| `context/vision.md` | Why we exist, where we're going (3-5+ years) | — | Strategy work |
| `context/strategy.md` | How we win (Narrative, Playing Field, Winning Moves) | context/vision.md | Roadmap work |
| `context/roadmap.md` | What we're building, in what order (point-in-time, dated) | context/vision.md, context/strategy.md | Prioritization, OKRs |

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

When `products/` folder exists, ask "Which product?" before proceeding.

### Other

| File | Purpose |
|------|---------|
| `sessions/` | Session summaries for memory |
| `uploads/` | User documents (pitch decks, etc.) |
| `templates/` | All templates (.template.md files) |

### File Creation Rules

**STRICT:** Only create files listed above.

When new content needs saving:
1. Check if existing file fits (user learnings → user-profile, company info → company-profile)
2. Merge into appropriate existing file
3. Never create new ad-hoc files

**No exceptions:**
- Not for "just this one case"
- Not for "temporary storage"
- Not because "it doesn't fit perfectly"
- If it doesn't fit listed files, ask user where it should go

**Why this matters:** Uncontrolled file creation creates sprawl. The system becomes unnavigable. Better to merge imperfectly than create file no one will find.

---

## How Context Gets Built

### First-Time Users (Empty Profiles)

**Step 1: User Context First (sets tone)**

Ask: "What's your role?" (senior PM, founder, engineer, etc.)

- If already a PM → skip familiarity question, proceed to company
- If not a PM → ask about PM familiarity (new / somewhat / very familiar)

Adapt communication style:
| Familiarity | Style |
|-------------|-------|
| New to PM | Educational, explain concepts |
| Somewhat familiar | Balanced, assume basics |
| Very familiar / Is PM | Direct, peer-level challenge |

**Step 2: Company Context (essential)**

Ask: "Do you have a company website I can look at?"

- If yes → fetch website, infer what you can, confirm with user
- If fetch fails → search company name for context
- If no website → offer: A) Upload files to `uploads/`, B) Quick interview, C) Skip

**Step 3: Answer Original Question**

With whatever context you have. If thin, flag it: "I don't have full context on your company stage, so I'll give options for different scenarios..."

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

Created through conversation. Manual creation not required.

→ Session format in `sessions/CLAUDE.md`
