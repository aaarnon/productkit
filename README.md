# PM-Copilot

Your AI product coach for strategy, discovery, roadmapping, and alignment.

**For:** Solo founders, PMs, CPOs, consultants, and anyone doing product work.

---

## Quick Start

1. Clone this repo
2. Set up your profiles:
   ```bash
   cd context
   cp company-profile.template.md company-profile.md
   cp user-profile.template.md user-profile.md
   cp product-profile.template.md product-profile.md
   ```
3. Open in Claude Code and describe your product challenge

Example prompts:
- "I need to prioritize my backlog but everything feels important"
- "Help me define our product strategy"
- "We're struggling to align stakeholders on our roadmap"

---

## How It Works

**Agents** = Domain coaches for extended conversations
**Skills** = Tools that produce specific outputs

| Agent | What It Does |
|-------|-------------|
| **Orchestrator** | Routes to agents, adapts to your expertise |
| **Vision** | Long-term purpose (3-5+ years) |
| **Strategy** | How to win, tactical choices |
| **Discovery** | Problem validation, opportunity mapping |
| **Roadmap** | Initiative planning, sequencing |
| **Metrics** | Success measurement, OKRs |
| **Stakeholder** | Coordination, alignment, RACI |

Agents suggest handoffs when appropriate. Example: After strategy work, you might hear "I recommend working with Discovery next to validate these assumptions."

---

## Key Frameworks

| Domain | Frameworks |
|--------|-----------|
| Strategy | DHM, Four Fits, Four Types of Work |
| Discovery | OST, 4 Risks, Confidence Scale |
| Roadmap | 6 Narrative Modes, Now-Next-Later |
| Metrics | AARRR, Impact Models, OKRs |
| Alignment | Product Operating Model, Red/Blue Phases |

See `knowledge/resources.md` for sources (Gibson Biddle, Teresa Torres, Brian Balfour, April Dunford, John Cutler, and more).

---

## Project Structure

```
pm-copilot/
├── agents/        # 7 agent definitions
├── skills/        # 11 utility skills
├── knowledge/     # 55+ framework articles
├── context/       # Your profiles, sessions, uploads
├── outputs/       # Generated work (one-pagers, roadmaps, OKRs)
└── extra/         # Personality (PM jokes)
```

---

## Privacy

Your data stays local. The `.gitignore` excludes all user-specific content:
- `context/*.md` — Your filled profiles (templates are shared)
- `context/sessions/*` — Your conversation history
- `context/uploads/*` — Your uploaded documents
- `outputs/*` — Your generated work products

System files (agents, skills, knowledge) are shared.

---

## Contributing

Contributions welcome:
- Knowledge base articles
- Framework refinements
- Agent behavior improvements
- New utility skills

---

## License

Open source. See LICENSE file.
