# ProductKit

ProductKit is a context-aware system for product management, featuring composable skills for strategy, discovery, roadmapping, and prioritization.

---

## Overview

Software engineers have [SpecKit](https://github.com/github/spec-kit), [BMAD](https://github.com/bmadcode/BMAD-METHOD), or [Superpowers](https://github.com/obra/superpowers) for context-driven development. Product managers? Unstructured chats with LLMs that lead to generic advice.

Ask ChatGPT "how should I prioritize my backlog?" and you'll get a textbook answer about RICE scoring - regardless of whether you're pre-PMF or Series C, B2B or B2C, a team of 3 or 300.

However, [product management is business management](https://swkhan.medium.com/product-management-is-business-management-why-does-everyone-forget-that-85f777da30e1). The right approach depends entirely on context: company stage, business model, team structure, current challenges. Without that context, advice is noise.

ProductKit solves this by:
1. **Building context first** - Company stage, business model, user profile
2. **Routing to specialists** - Domain-expert agents for strategy, discovery, metrics, etc.
3. **Producing deliverables** - Not just advice, but actual artifacts: roadmaps, OKRs, one-pagers, strategy docs
4. **Verifying quality** - Every deliverable runs through explicit checks before delivery (inspired by engineering test patterns)

---

## Quick Start

**Option 1** - In your AI coding agent (Claude Code, Cursor, Codex, etc.):

```
Let's clone

https://github.com/aaarnon/productkit

into a new top-level directory in this project called "productkit/"
```

**Option 2** - [Download ZIP from GitHub](https://github.com/aaarnon/productkit/archive/refs/heads/main.zip) and extract to your project.

### Activate ProductKit

After cloning, activate ProductKit by running this prompt:

```
Read productkit/CLAUDE.md and start a session.
```

If working, ProductKit will introduce itself and begin onboarding.

### Setup by AI Tool

ProductKit uses `CLAUDE.md` files as the standard. Why Claude? As of this writing, Claude seems best suited for back-and-forth conversations, which ProductKit relies on. Tools like Codex and Gemini appear better for one-shot solutions. This is just the author's observation, so feel free to choose your preferred tool.

Other CLIs and IDEs can read these files via fallback config.

--

**Claude Code** - Full skill auto-discovery. Optimal experience. No setup needed.

--

**Cursor** - after cloning, run this prompt in Cursor:
```
Create an AGENTS.md file in the project root with this content:

Always read and follow productkit/CLAUDE.md before responding.
```

--

**Codex** - after cloning, run this prompt in Codex:
```
Update ~/.codex/config.toml to add a per-project entry for the current working
directory with project_doc_fallback_filenames = ["CLAUDE.md"], leaving global
defaults unchanged. If the project entry doesn't exist, create it.
```

--

**Gemini CLI** - after cloning, run this prompt in Gemini:
```
Update or create the project-specific settings file located at .gemini/settings.json in the current
directory. Ensure the JSON contains a "context" object with a "fileName" array set to ["CLAUDE.md",
"GEMINI.md"]. Preserve any other existing settings in the file.
```

--

---

## Updates

ProductKit checks for updates automatically at the start of each session and notifies you if a new version is available.

To update:

```bash
cd productkit && git pull
```

Your data in `context/` and `outputs/` stays untouched.

---

## How It Works

**Skills** are specialized capabilities that handle different PM domains (strategy, discovery, metrics, etc.). Each skill knows its domain deeply and produces specific deliverables.

**Knowledge** is the source material (from John Cutler, Teresa Torres, Tim Herbig, April Dunford, Brian Balfour, and other product legends).

**Context** stores your company profile, user profile, and strategic foundation (vision → strategy → metrics → discovery → roadmap).

```
┌────────────────────────────────────────────────────────────────┐
│                                                                │
│   User Question                                                │
│        ↓                                                       │
│   ┌─────────────┐    checks    ┌─────────────┐                 │
│   │  AI Tool    │ ──────────→  │   Context   │                 │
│   │ (Claude,    │              │  (profiles) │                 │
│   │  Cursor...) │              └─────────────┘                 │
│   └─────────────┘                                              │
│        │ triggers matching skill                               │
│        ↓                                                       │
│   ┌─────────────┐    uses     ┌─────────────┐                  │
│   │   Skill     │ ──────────→ │  Knowledge  │                  │
│   │ (Strategy,  │             │  base       │                  │
│   │  Discovery, │             └─────────────┘                  │
│   │  Metrics...)│                                              │
│   └─────────────┘                                              │
│        │                                                       │
│        ↓                                                       │
│   ┌─────────────┐                                              │
│   │ Verification│ - Checks quality criteria                    │
│   │  (Auto)     │ - Iterates until standards met               │
│   │             │ - Shows transparent progress                 │
│   └─────────────┘                                              │
│        │                                                       │
│        ↓                                                       │
│   Deliverable (roadmap, one-pager, OKRs, strategy doc, etc.)   │
│   + Eval Summary (what passed, what needed work)               │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

### Quality Verification

Unlike generic AI that says "here's your roadmap" and stops, ProductKit verifies deliverables before presenting them.

**How verification works:**
1. After you approve ("Ready to create the roadmap?"), ProductKit generates a draft
2. Runs verification checks automatically (structural requirements + quality standards)
3. Failed checks trigger regeneration (asks for your input if needed)
4. You see transparent progress: "Checking metric linkage... ✗ Missing. Regenerating..."
5. Delivers final output with an Eval Summary showing all checks



---

## Workflow

1. **Start a conversation** - Describe your product challenge
2. **Build context** (first time) - ProductKit asks about your role and company
3. **Get matched** - AI tool triggers the right skill based on your intent
4. **Work iteratively** - Conversation toward a deliverable
5. **Produce output** - Skill generates artifacts (roadmap, OKRs, one-pager, etc.)
6. **Save session** (optional) - Preserve context for future conversations

### Skills Network

Skills reference each other based on domain. For example, strategy skill may suggest using discovery skill if assumptions need validation.

```mermaid
flowchart TB
    U((User)) <--> AI{AI Tool}
    AI <-.->|checks| C[(Context)]

    AI --> V[Vision]
    V --> S[Strategy]
    S --> D[Discovery]
    S --> M[Metrics]
    D --> R[Roadmap]
    M --> R
    R --> ST[Stakeholder]

    V & S & D & R & M & ST --> Out>Deliverable]
    Out --- E1[Roadmap]
    Out --- E2[OKRs]
    Out --- E3[One-pager]
    Out --- E4[Strategy doc]
```

### Example: Foundation Check

```
User: "Help me create a strategy one-pager"
                         ↓
   ProductKit checks: Do we have a product vision?
                         ↓
         ┌───────────────┴───────────────┐
         ↓                               ↓
        NO                              YES
         ↓                               ↓
"Vision missing.            Check: Do we have a strategy?
Your call:                               ↓
A) Build vision first               ┌────┴────┐
B) Proceed anyway"                  ↓         ↓
         ↓                         NO        YES
    User decides                    ↓         ↓
         ↓               "Strategy missing.    Generate output from
If A → Vision skill       Your call:           existing strategy
If B → Proceed            A) Build strategy
       with gaps          B) Proceed anyway"
```

### Example: Skill Conversation

```
YOU: "I need to prioritize my backlog but everything feels important"

PRODUCTKIT: "What's your role and experience level?"
YOU: "Senior PM, 5 years"

PRODUCTKIT: "Got it. What stage is your company?
             And what deliverable do you want to walk away with?"
YOU: "Series A, post-PMF. I need a prioritized roadmap for Q1."

PRODUCTKIT: "Sounds like you're in execution mode. Let's check if
             priorities should be obvious from your strategy. If not,
             we'll fix that first."

[Strategy skill activates]

PRODUCTKIT: "What's your current product strategy? If prioritization
             feels hard, the strategy might be unclear."
YOU: "We're trying to increase activation and reduce churn"

PRODUCTKIT: "Those are two different bets. Which matters more right now?"
YOU: "Activation. We're leaking users in onboarding"

PRODUCTKIT: "Clear. With activation as the focus, let's build your Q1
             roadmap. I'll use Now-Next-Later format. What are your
             top 3 activation problems?"

[Roadmap skill activates]

... conversation continues.
```

---

## Philosophy

**→ Context over generic advice.**
The same question deserves different answers at different company stages. Pre-PMF needs speed and learning. Post-PMF needs structure and alignment. ProductKit asks first, advises second.

**→ Deliverables over opinions.**
Great PMs ship artifacts that align teams: roadmaps, OKRs, one-pagers, strategy docs. Every conversation should move toward something concrete.

**→ Challenge over agreement.**
Weak thinking produces weak products. ProductKit pushes back on unclear strategy, unreasonable scope, and unvalidated assumptions. Honest feedback beats comfortable agreement.

**→ Perspectives over prescriptions.**
The knowledge base includes diverse (sometimes conflicting) viewpoints. Great PMs don't always agree. That's intentional - PM work is contextual, not formulaic.

---

## Project Structure

```
productkit/
├── skills/      # Composable skills (strategy, discovery, metrics, etc.)
├── knowledge/   # Articles from product thought leaders
├── context/     # Your data: profiles, foundations, sessions (gitignored)
│   └── templates/  # Templates (git tracked)
└── outputs/     # Generated deliverables (gitignored)
```

**Privacy:** Your data stays local. `context/` and `outputs/` are gitignored.

---

## Attribution

ProductKit's knowledge base includes publicly available content from product thought leaders: Teresa Torres, John Cutler, Gibson Biddle, Marty Cagan, April Dunford, Brian Balfour, and others. Their frameworks and insights power the coaching this system provides.

We support these authors by crediting them in conversation, attributing frameworks in deliverables, and recommending their books, courses, and newsletters, helping them reach new audiences and monetize their work.

For the full author directory with links to their original content, see `knowledge/authors.md`.

---

## Contributing

Contributions welcome. Suggest new features, report bugs, propose different skills or workflows. Open an issue or submit a PR.

---

## License

MIT License. See [LICENSE](LICENSE).
