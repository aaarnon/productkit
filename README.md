# PM-Copilot

Your AI product coach for strategy, discovery, roadmapping, and alignment.

**For:** Solo founders, PMs, CPOs, consultants, and anyone doing product work.

---

## Quick Start

### Option 1: Have your AI coding agent clone it into your project

Create a new directory for your project and open it in your AI coding agent (Claude Code, Cursor, Gemini CLI, Codex, etc.).

Tell your AI coding agent:

```
Let's clone

https://github.com/aaarnon/pm-copilot

into a new top-level directory in this project called "pm-copilot/"
```

### Option 2: Download as ZIP and drag into your project

[Download the ZIP from GitHub](https://github.com/aaarnon/pm-copilot/archive/refs/heads/main.zip) and drag the `pm-copilot` folder into your project directory.

---

Once integrated, reference the files with `@pm-copilot/` mentions or just start chatting.

On your first message, the Orchestrator will:
- Ask about your role and experience (to set the right tone)
- Help you build a company profile (essential for relevant advice)
- Then dive into your question

**Example prompts:**
- "I need to prioritize my backlog but everything feels important"
- "Help me define our product strategy"
- "We're struggling to align stakeholders on our roadmap"

---

## How It Works

### Focused on PM Deliverables

Great product managers ship deliverables, not just opinions. Strategy docs, roadmaps, one-pagers, OKRs - these artifacts align teams, secure buy-in, and drive execution.

PM-Copilot helps you produce these deliverables. Every conversation aims toward a concrete output.

### Agents & Skills

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

### Example Interaction

```
YOU: "I need to prioritize my backlog but everything feels important"

ORCHESTRATOR: "What's your role and experience level?"
YOU: "Senior PM, 5 years"

ORCHESTRATOR: "Got it. Quick context - what stage is your company?
              And what deliverable do you want to walk away with today?"
YOU: "Series A, post-PMF. I need a prioritized roadmap for Q1."

ORCHESTRATOR: "Sounds like you're in execution mode. Let me hand you
              to Strategy to check if priorities should be obvious
              from your strategy. If not, we'll fix that first."

STRATEGY: "What's your current product strategy? If prioritization
          feels hard, the strategy might be unclear."
YOU: "We're trying to increase activation and reduce churn"

STRATEGY: "Those are two different bets. Which matters more right now?
          Gibson Biddle would say: if you can't prioritize, your
          strategy isn't sharp enough."
YOU: "Activation - we're leaking users in onboarding"

STRATEGY: "Clear. I'll hand you to Roadmap agent with this context."

ROADMAP: "Based on activation focus, let's build your Q1 roadmap.
         I'll use the Now-Next-Later format. What are your top 3
         activation problems?"

→ Delivers: Prioritized Q1 roadmap document
```

Agents suggest handoffs when appropriate and always aim toward a deliverable.

This isn't "ChatGPT for PMs." It's a **system** - like [SpecKit](https://github.com/CodingBull-dev/speckit) or [BMAD](https://github.com/bmadcode/BMAD-METHOD) for engineers, but for Product Managers. It remembers your context, challenges your thinking, and brings structure to the messy middle where vision, strategy, and execution need to connect.

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
- `context/*.md` - Your filled profiles (templates are shared)
- `context/sessions/*` - Your conversation history
- `context/uploads/*` - Your uploaded documents
- `outputs/*` - Your generated work products

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

MIT License. See [LICENSE](LICENSE).
