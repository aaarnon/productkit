# Decision Log

Decisions made during the initial project definition conversation.

---

## Project Scope

### Decision: Broad scope with modular design (Option A)
**Context:** Arnon considered whether to focus on one specific use case (e.g., just roadmapping) or keep the scope broad covering Discovery, Strategy, and Roadmap.

**Decision:** Keep broad scope because these areas are interconnected - you can't have a good roadmap without strategy, can't have strategy without understanding customers.

**Boundary defined:**
- **IN scope:** Discovery, Strategy, Planning/Roadmap, Metrics
- **OUT of scope:** Delivery (sprints, tickets, execution), Resource allocation, Budget planning

---

## Target Users

### Decision: All product personas, agent adapts
**Context:** Considered whether to target solo founders, experienced PMs, or team leads.

**Decision:** Support all personas. The Orchestrator agent detects experience level and adapts guidance accordingly.

---

## Deliverables

### Decision: Multiple artifacts based on user needs
**Context:** Considered whether the output should be a single document or multiple formats.

**Decision:** Flexible output - the agent produces what the user asks for (vision statement, strategy doc, roadmap, OKRs, etc.)

---

## Framework Reference

### Decision: Use PM deliverables framework as guide
**Context:** Arnon shared a visual framework showing the relationship between PM deliverables.

**Reference:** See `pm-deliverables.png` in this folder.

**Framework rows:**
1. Vision Statement - "Where do we want to go?"
2. Strategy Document - "How will we get there?"
3. Product Roadmap - "What milestones?" (includes Problem Framing, Solution Framing, Prioritization)
4. Deliver Solution - OUT OF SCOPE
5. Insights/Metrics - "How do we know we're making progress?"

---

## Agent Architecture

### Decision: Hybrid model with Orchestrator + Specialists
**Context:** Considered three options:
- A) Domain agents (OKR Agent, Prioritization Agent, etc.) - horizontal
- B) Phase agents (Interviewer → Strategist → Planner) - vertical
- C) Hybrid (Orchestrator + domain specialists)

**Decision:** Hybrid model. One Orchestrator handles interview and routing, specialists go deep when needed. Mirrors how a real product consultancy works.

---

### Decision: Alignment as separate agent
**Context:** Considered whether Alignment should be part of Roadmap agent or separate.

**Decision:** Separate agent because:
- Alignment is a communication/influence problem, not a planning problem
- Different skills needed (stakeholder mapping, objection handling)
- Can be invoked across multiple domains (Vision alignment, Strategy alignment, Roadmap alignment)

---

### Decision: 7 main agents + 4 utility skills
**Context:** Defined the full agent architecture.

**Main agents (entry points):**
1. Orchestrator - interviews, detects intent, routes
2. Vision - "Where do we want to go?"
3. Strategy - "How will we get there?" (includes positioning)
4. Discovery - Problem/Solution framing, opportunities
5. Roadmap - Prioritization, sequencing, timelines
6. Metrics - OKRs, success measures, feedback loops
7. Alignment - Stakeholder buy-in (horizontal, serves all)

**Utility skills (composable):**
1. Prioritization - RICE, urgency, value/effort frameworks
2. Positioning - April Dunford framework
3. Opportunity Tree - Teresa Torres OST
4. OKR Builder - OKR creation helper

---

## Folder Structure

### Decision: Skills-based structure with agents and utilities separation
**Context:** Considered how to organize for Claude Code integration and open source contribution.

**Final structure:**
```
roadmap-product/
├── .claude/skills/
│   ├── agents/           # 7 main agents
│   └── utilities/        # 4 composable helpers
├── knowledge/            # Best practices per domain
├── templates/            # Deliverable templates
├── examples/             # Sample outputs by industry
└── docs/                 # Documentation
```

**Rationale:**
- Native Claude Code skills integration
- Clear separation between agents (entry points) and utilities (composable)
- Knowledge base separate from skills for easier maintenance
- Examples help users understand expected output

---

## Inspirations

### Decision: Draw from BMAD, Ideation Agent, and From-Thinking-to-Coding
**Context:** Arnon shared reference projects to learn from.

**Key patterns adopted:**
- From BMAD: Multi-agent architecture, specialized roles
- From Ideation Agent: Phase-based workflow, CLI interview approach
- From From-Thinking-to-Coding: Conversational interviewing, templates per phase

---

## Philosophy

### Decision: Frameworks as mental models, not rigid templates
**Context:** Referenced Ant Murphy's article about breaking frameworks.

**Principle:** The agent should teach and apply frameworks but adapt to context. Use frameworks as thinking tools, not prescriptive formulas.

---

## Claude Code Integration

### Decision: No AGENTS.md file
**Context:** AGENTS.md is used by other AI coding tools (Cursor, Windsurf) but not Claude Code.

**Decision:** Don't use AGENTS.md. Claude Code uses:
- `CLAUDE.md` files for memory/instructions
- Skills with YAML frontmatter for auto-discovered tools
- Subagents via Task tool for parallel isolated work

---

### Decision: agents/ folder contains mode definitions, not real subagents
**Context:** Clarified that files in `agents/` are instruction documents, not Claude Code subagents.

**Decision:** The `agents/*.md` files are "mode definitions" that Claude reads when entering a domain. They work because root `CLAUDE.md` references them. Real subagents (via Task tool) spawn isolated Claude instances — different pattern.

---

### Decision: Folder-level CLAUDE.md pattern
**Context:** Decided how to organize instructions across the project.

**Decision:** Use CLAUDE.md at multiple levels:
- Root `CLAUDE.md` — project overview
- `knowledge/CLAUDE.md` — how knowledge files work
- `skills/CLAUDE.md` — how skills work

No need for SKILL.md or AGENTS.md in root — current structure is sufficient.

---

### Decision: resources.md lives in knowledge/
**Context:** Considered whether resources.md belongs at root or in knowledge folder.

**Decision:** Move to `knowledge/resources.md` because:
- It's a catalog OF the knowledge base
- Pairs with `knowledge/CLAUDE.md` (how it works + what's in it)
- Root should have project-level files only (CLAUDE.md, README.md, decisions.md)

---

### Decision: Agents use YAML frontmatter (like skills)
**Context:** Considered whether agent files should use YAML frontmatter for consistency with skills.

**Decision:** Yes, add YAML frontmatter to all agent files:
```yaml
---
name: agent-name
description: What it does + when to use it.
---
```

**Rationale:**
- Consistency with skills pattern
- Enables auto-discovery via description matching
- Claude Code can match user prompts to agent descriptions
- Files remain .md (Obsidian compatible) — YAML is just a header block

---

### Decision: Knowledge files don't need YAML frontmatter
**Context:** Considered whether knowledge files should also use YAML like skills and agents.

**Decision:** No — current markdown header format is sufficient:
```markdown
# Title
**Source:** Author
**URL:** https://...
**Use in:** Agent, Skill
```

**Rationale:**
- Knowledge files are not "triggered" — they're searched/read by agents when needed
- Current format already captures metadata (source, author, used by)
- YAML would add complexity without enabling new functionality
- Skills/agents need YAML for auto-discovery; knowledge files don't

---

### Decision: Project renamed to PM-Copilot
**Context:** "Roadmap Product" was too generic and descriptive. Needed something more memorable.

**Decision:** Renamed to **PM-Copilot**

**Rationale:**
- Straightforward — clearly says what it is
- Clear audience — PMs
- Action-oriented — "Copilot" implies assistance, not replacement
- Folder can be renamed from `roadmap-product/` to `pm-copilot/` later

---

### Decision: README optimized for quick scanning
**Context:** Original README was 355 lines — too long for GitHub visitors.

**Decision:** Rewrote to ~90 lines following best practices:
- Lead with value proposition (what it does, who it's for)
- Quick Start section early (3 steps + example prompts)
- Tables instead of prose for reference content
- Details moved to folder-level CLAUDE.md files

**Rationale:**
- GitHub visitors decide in seconds whether to engage
- Main idea first, details later
- Quick Start enables immediate use without reading everything
