# PM-Copilot

The "SpecKit" for product management. PM-Copilot is a multi-agent system that understands your product context before guiding you through strategy, discovery, roadmapping, and prioritization. 

**For:** Engineers, PMs, founders, or any operator working in the product management context.

---

## Overview

Software engineers have [SpecKit](https://github.com/AviCraworker/speckit), [BMAD](https://github.com/bmadcode/BMAD-METHOD), or [Claude Superpowers](https://github.com/aaronsb/claude-superpowers) for context-engineered development. Product managers? Unstructured chats with LLMs that lead to generic advice.

Ask ChatGPT "how should I prioritize my backlog?" and you'll get a textbook answer about RICE scoring - regardless of whether you're pre-PMF or Series C, B2B or B2C, a team of 3 or 300.

Product management is business management. The right approach depends entirely on context: company stage, business model, team structure, current challenges. Without that context, advice is noise.

PM-Copilot solves this by:
1. **Building context first** - Company stage, business model, user profile
2. **Routing to specialists** - Domain-expert agents for strategy, discovery, metrics, etc.
3. **Producing deliverables** - Not just advice, but actual artifacts: roadmaps, OKRs, one-pagers, strategy docs

---

## Quick Start

### Option 1: Clone via AI coding agent

In your AI coding agent (Claude Code, Cursor, Codex, etc.):

```
Let's clone

https://github.com/aaarnon/pm-copilot

into a new top-level directory in this project called "pm-copilot/"
```

### Option 2: Download manually

[Download ZIP from GitHub](https://github.com/aaarnon/pm-copilot/archive/refs/heads/main.zip) and extract to your project.

### Verify

Reference files with `@pm-copilot/` mentions or start chatting. The Orchestrator will introduce itself.

### Using a Different AI Tool

This project was built for Claude Code, but works with any AI coding tool.

The `CLAUDE.md` files provide AI context. If using a different tool, create symlinks to your tool's config filename:

```bash
# From pm-copilot directory - replace TARGET with your tool's config filename
find . -name "CLAUDE.md" -exec sh -c 'ln -sf CLAUDE.md "$(dirname "$1")/TARGET"' _ {} \;
```

| Tool | Target Filename | Command |
|------|-----------------|---------|
| Gemini CLI | GEMINI.md | `find . -name "CLAUDE.md" -exec sh -c 'ln -sf CLAUDE.md "$(dirname "$1")/GEMINI.md"' _ {} \;` |
| Codex | AGENTS.md | `find . -name "CLAUDE.md" -exec sh -c 'ln -sf CLAUDE.md "$(dirname "$1")/AGENTS.md"' _ {} \;` |
| Cursor | .cursorrules | `ln -sf CLAUDE.md .cursorrules` (root only) |
| Antigravity | Check docs | Replace TARGET in command above |

---

## How It Works

**Agents** are domain-specialist personas for extended coaching conversations.

**Skills** are discrete tools that produce specific outputs.

**Knowledge** is the source material (from John Cutler, Teresa Torres, Tim Herbig, April Dunford, Brian Balfour, and others product legends).

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│   User Question                                                │
│        ↓                                                       │
│   ┌─────────────┐    checks    ┌─────────────┐                 │
│   │ Orchestrator│ ──────────→  │   Context   │                 │
│   └─────────────┘              │  (profiles) │                 │
│        │                       └─────────────┘                 │
│        │ routes to specialist                                  │
│        ↓                                                       │
│   ┌─────────────┐    uses     ┌─────────────┐                  │
│   │   Agent     │ ──────────→ │  Knowledge  │                  │
│   │ (Strategy,  │             │  base       │                  │
│   │  Discovery, │             └─────────────┘                  │
│   │  Metrics...)│                                              │
│   └─────────────┘                                              │
│        │                                                       │
│        │ invokes                                               │
│        ↓                                                       │
│   ┌─────────────┐                                              │
│   │   Skills    │ ──────────→  Deliverable                     │
│   │ (OKR,       │              (roadmap, one-pager, etc.)      │
│   │  prioritize)│                                              │
│   └─────────────┘                                              │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```



---

## Agent Handoffs

### Workflow

1. **Start a conversation** - Describe your product challenge
2. **Build context** (first time) - Orchestrator asks about your role and company
3. **Get routed** - Orchestrator hands off to the right specialist agent
4. **Work with the agent** - Iterative conversation toward a deliverable
5. **Produce output** - Agent invokes skills to generate artifacts
6. **Save session** (optional) - Preserve context for future conversations

### Routing

Agents hand off to each other based on domain. Orchestrator coordinates all routing.

```mermaid
flowchart TB
    U((User)) <--> O{Orchestrator}
    O <-.->|context| C[(Context)]

    O <--> V[Vision]
    O <--> S[Strategy]
    O <--> D[Discovery]
    O <--> R[Roadmap]
    O <--> M[Metrics]
    O <--> ST[Stakeholder]

    V <-.-> S
    S <-.-> D
    S <-.-> R
    D <-.-> R
    R <-.-> M
    M <-.-> ST

    S & D & R & M <-->|skills| SK[[Skills]]
    SK --> Out>Deliverable]
    Out --- E1[Roadmap]
    Out --- E2[OKRs]
    Out --- E3[One-pager]
    Out --- E4[Strategy doc]
```

### Example: Orchestrator → Strategy → Roadmap

```
YOU: "I need to prioritize my backlog but everything feels important"

ORCHESTRATOR: "What's your role and experience level?"
YOU: "Senior PM, 5 years"

ORCHESTRATOR: "Got it. What stage is your company?
              And what deliverable do you want to walk away with?"
YOU: "Series A, post-PMF. I need a prioritized roadmap for Q1."

ORCHESTRATOR: "Sounds like you're in execution mode. Let me hand you
              to Strategy agent to check if priorities should be obvious
              from your strategy. If not, we'll fix that first."

STRATEGY: "What's your current product strategy? If prioritization
          feels hard, the strategy might be unclear."
YOU: "We're trying to increase activation and reduce churn"

STRATEGY: "Those are two different bets. Which matters more right now?"
YOU: "Activation. We're leaking users in onboarding"

STRATEGY: "Clear. I'll hand you to Roadmap agent with this context."

ROADMAP: "Based on activation focus, let's build your Q1 roadmap.
         I'll use Now-Next-Later format. What are your top 3
         activation problems?"

... conversation continues.
```


---

## Philosophy

**→Context over generic advice**
The same question deserves different answers at different company stages. Pre-PMF needs speed and learning. Post-PMF needs structure and alignment. PM-Copilot asks first, advises second.

**→ Deliverables over opinions**
Great PMs ship artifacts that align teams: roadmaps, OKRs, one-pagers, strategy docs. Every conversation should move toward something concrete.

**→ Challenge over agreement**
Weak thinking produces weak products. PM-Copilot pushes back on unclear strategy, unreasonable scope, and unvalidated assumptions. Honest feedback beats comfortable agreement.

**→ Perspectives over prescriptions**
The knowledge base includes diverse (sometimes conflicting) viewpoints. Great PMs don't always agree. That's intentional - PM work is contextual, not formulaic.

---

## Project Structure

```
pm-copilot/
├── agents/      # Specialist agents (orchestrator, strategy, discovery, etc.)
├── skills/      # Output-producing tools (prioritization, okr-builder, etc.)
├── knowledge/   # Source articles by domain (strategy, discovery, metrics, etc.)
├── context/     # Your data - profiles, sessions, uploads (gitignored)
├── outputs/     # Generated deliverables (gitignored)
└── extra/       # Personality (PM jokes)
```

**Privacy:** Your data stays local. `context/` and `outputs/` are gitignored. System files are shared, your data is not.

---

## Contributing

Contributions welcome:
- Knowledge base articles (new frameworks, authors)
- Agent behavior improvements
- New utility skills
- Bug fixes and refinements

---

## License

MIT License. See [LICENSE](LICENSE).
