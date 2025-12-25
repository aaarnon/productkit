# Roadmap Product - Detailed Implementation Plan

**Created:** December 25, 2025
**Last Updated:** December 25, 2025
**Status:** Phase 2 In Progress - Testing & Refining

---

## Executive Summary

### Project Goal
Build an open-source multi-agent system that helps product teams with strategy, discovery, roadmapping, and alignment work.

### Current State
- **Definition Phase:** COMPLETE
- **Knowledge Base:** COMPLETE (38 files)
- **Agent Definitions:** COMPLETE (7 agents)
- **Utility Skills:** COMPLETE (11 skills)
- **Context System:** COMPLETE (company + user profiles)
- **Implementation:** IN PROGRESS (simplified markdown-based approach)
- **Testing:** STARTED (real-world testing with user scenarios)

### Key Finding
The project is **architecturally coherent** and has been **simplified**. Instead of complex SDK/MCP implementations, agents are markdown files that Claude reads directly. This enables faster iteration and keeps the project accessible to non-developers.

---

## Project Inventory

### Files Created

| Category | Count | Status |
|----------|-------|--------|
| Agent definitions | 7 | Complete |
| Utility skills | 11 | Complete |
| Knowledge files | 38 | Complete |
| Context files | 3 | Complete |
| Documentation | 3 | Complete |
| CLAUDE.md files | 5 | Complete |
| Extra files | 1 | Complete |
| **Total** | **68** | **Complete** |

### Verification Results

- [x] All knowledge file references in agents exist
- [x] All neighbor relationships are bidirectional
- [x] All utility skills referenced are implemented
- [x] All frameworks are documented
- [x] No orphaned or broken references

---

## Phase 1: Definition (COMPLETE)

### 1.1 Agent Definitions
- [x] Orchestrator agent - Central coordinator, context management, 360 coherence
- [x] Vision agent - Long-term purpose (3-5+ years)
- [x] Strategy agent - How to win
- [x] Discovery agent - Problem validation
- [x] Roadmap agent - Initiative planning
- [x] Metrics agent - Success measurement
- [x] Stakeholder agent - Stakeholder coordination (renamed from Alignment)

### 1.2 Utility Skills
- [x] skill-creator - Template for creating new skills
- [x] Prioritization - VEUC, DHM, "priority should be obvious"
- [x] Positioning - April Dunford's 5-step exercise
- [x] Opportunity-tree - OST creation and prioritization
- [x] OKR-builder - Objectives and Key Results
- [x] Impact-model-builder - Driver trees
- [x] Metric-selector - Choose right metrics
- [x] Leading-lagging-mapper - Indicator relationships
- [x] AARRR-analyzer - Pirate metrics funnel
- [x] Initiative-alignment-doc - Product Alignment Document (renamed from one-pager)
- [x] Interview-summary - Customer interview synthesis

### 1.3 Knowledge Base
- [x] Strategy folder (7 files)
- [x] Discovery folder (9 files)
- [x] Roadmap folder (5 files)
- [x] Metrics folder (5 files)
- [x] Alignment folder (10 files)
- [x] Prioritization folder (2 files)

### 1.4 Context System
- [x] context/CLAUDE.md - Context rules
- [x] context/company-profile.md - Company context template
- [x] context/user-profile.md - User context template
- [x] context/uploads/ - Folder for user documents

### 1.5 Templates
- [x] Product Alignment Document (operational template)
- [x] How to Use Product Alignment Doc (guidance)

### 1.6 Personality & Extras
- [x] extra/pm-jokes.md - PM humor for conversations

### 1.7 Documentation
- [x] README.md - Project overview
- [x] resources.md - Source articles and references
- [x] detailed-plan.md - This file

---

## Phase 2: Implementation (IN PROGRESS)

This phase transforms definitions into working AI agents.

### 2.1 Technical Architecture Decision
- [x] **Implementation platform chosen: Simplified Markdown-Based Approach**
  - Agents are markdown files that Claude reads directly
  - No SDK, MCP, or custom framework needed
  - Orchestrator in CLAUDE.md handles routing
  - Skills are markdown files with YAML frontmatter
  - Knowledge files loaded on-demand

**Why this approach:**
- Simpler than SDK/MCP alternatives
- Accessible to non-developers
- Fast iteration and testing
- Agents already ARE the system prompts
- Context stays in conversation window

### 2.2 Agent Definitions (Complete - agents ARE their prompts)

With simplified approach, agent markdown files serve as system prompts:
- [x] All 7 agents have complete definitions
- [x] Knowledge base references included
- [x] Neighbor awareness documented
- [x] Output formats specified
- [x] Common pitfalls listed

**Orchestrator enhancements (done):**
- [x] Context check flow (company + user profiles)
- [x] Red/Blue phase diagnosis with explanation
- [x] Product coherence check (360 view)
- [x] Deliverable question before routing
- [x] Context update suggestions
- [x] Web search for company context building

### 2.3 Utility Skill Implementation (Complete)

All skills have YAML frontmatter with description for triggering:
- [x] skill-creator (meta template)
- [x] Prioritization (hybrid)
- [x] Positioning (hybrid)
- [x] Opportunity-tree (agent-called)
- [x] OKR-builder (agent-called)
- [x] Impact-model-builder (agent-called)
- [x] Metric-selector (agent-called)
- [x] Leading-lagging-mapper (agent-called)
- [x] AARRR-analyzer (agent-called)
- [x] Initiative-alignment-doc (agent-called)
- [x] Interview-summary (agent-called)

### 2.4 Inter-Agent Communication (Simplified)

With markdown approach, handoffs are conversational:
- [x] Orchestrator reads agent files as needed
- [x] Handoffs happen by reading new agent file
- [x] Context stays in conversation
- [x] No external state management needed

---

## Phase 3: Testing & Validation (IN PROGRESS)

### 3.1 Unit Testing (Per Agent)
For each agent, test:
- [ ] Knowledge retrieval accuracy
- [ ] Framework application correctness
- [ ] Output format compliance
- [ ] Neighbor awareness triggers
- [ ] Edge case handling

### 3.2 Integration Testing
- [ ] Orchestrator → Vision handoff
- [ ] Vision → Strategy handoff
- [ ] Strategy → Discovery handoff
- [ ] Strategy → Metrics handoff
- [ ] Discovery → Roadmap handoff
- [x] Discovery → Metrics handoff (tested)
- [x] Roadmap → Stakeholder handoff
- [x] Roadmap → Metrics handoff (tested)
- [x] Metrics → Discovery handoff (tested)
- [ ] Stakeholder → Roadmap handoff
- [ ] Full workflow: Vision → Strategy → Discovery → Roadmap → Stakeholder

### 3.3 User Journey Testing
Test complete user scenarios:

#### Journey 1: Starting from Scratch
- [ ] New founder, no strategy
- [ ] Orchestrator diagnoses Blue phase
- [ ] Vision → Strategy → Discovery → Roadmap flow
- [ ] Appropriate depth per user expertise

#### Journey 2: Existing Strategy, Need Roadmap
- [ ] PM with clear strategy
- [ ] Orchestrator validates existing work
- [ ] Roadmap → One-pager → Alignment flow

#### Journey 3: Prioritization Problem
- [ ] Team with too many options
- [ ] Orchestrator identifies strategy problem
- [ ] Strategy → Prioritization utility flow

#### Journey 4: Metrics Setup
- [ ] Team needs success measurement
- [ ] Metrics agent with utility skills
- [ ] Impact model → OKR → Metric selection flow

### 3.4 Edge Case Testing
- [ ] User changes mind mid-flow
- [ ] Contradictory inputs from user
- [ ] Missing information handling
- [ ] Very early stage (no strategy, no vision)
- [ ] Very late stage (just needs execution help)
- [ ] Non-PM users (founders, engineers)
- [ ] CPO-level users (high-level only)

---

## Phase 4: Refinement (IN PROGRESS)

### 4.1 Prompt Optimization
Based on testing results:
- [x] Orchestrator explains Red/Blue after diagnosis
- [x] One question at a time (conversational)
- [x] Deliverable question scopes conversation
- [ ] Reduce hallucinations
- [ ] Improve framework adherence
- [ ] Optimize context usage

### 4.2 Knowledge Base Gaps
Identified during testing:
- [x] User interview techniques (added to Discovery)
- [x] Synthesis methods (interview-summary skill)
- [ ] Missing framework documentation
- [ ] Incomplete examples

### 4.3 User Experience
- [x] Conversation flow improvements (one question at a time)
- [x] Added personality (PM jokes)
- [x] Context building for tailored advice
- [ ] Better summarization
- [ ] Clearer next step guidance

---

## Phase 5: Deployment (NOT STARTED)

### 5.1 Packaging
- [ ] Create installation instructions
- [ ] Configuration documentation
- [ ] Environment requirements
- [ ] Dependency management

### 5.2 Documentation
- [ ] User guide
- [ ] Agent behavior reference
- [ ] Troubleshooting guide
- [ ] Contributing guide

### 5.3 Release
- [ ] Version 1.0 release
- [ ] GitHub repository setup
- [ ] License finalization
- [ ] Community announcement

---

## Known Gaps & Enhancements

### Current Gaps (To Address)

| Gap | Impact | Priority | Status |
|-----|--------|----------|--------|
| No implementation code | Blocking | High | Need to choose platform first |
| ~~Positioning utility lacks knowledge file~~ | ~~Low~~ | ~~Low~~ | **FILLED** - `product-positioning-april-dunford.md` |
| ~~OST full guide missing~~ | ~~Medium~~ | ~~Medium~~ | **FILLED** - `opportunity-solution-trees-teresa-torres.md` |
| ~~OKR Theatre article missing~~ | ~~Medium~~ | ~~Medium~~ | **FILLED** - `escape-okr-theatre-ant-murphy.md` |
| ~~VEUC framework missing~~ | ~~Medium~~ | ~~Medium~~ | **FILLED** - `veuc-prioritization-framework.md` |
| ~~User interview techniques~~ | ~~Low~~ | ~~Optional~~ | **FILLED** - `story-based-interviews-teresa-torres.md`, `continuous-interviewing-teresa-torres.md`, `no-time-for-discovery-teresa-torres.md` |
| ~~Research synthesis methods~~ | ~~Low~~ | ~~Optional~~ | **FILLED** - `interview-snapshot-teresa-torres.md` |

### Future Enhancements (Nice to Have)

| Enhancement | Description | Priority |
|-------------|-------------|----------|
| **Glossary** | Index of terms across knowledge base | Low |
| **Quick reference cards** | One-page summaries per agent | Low |
| **Video links** | Author talks and presentations | Low |
| **Industry templates** | SaaS, marketplace, B2B, B2C variants | Medium |
| **Integration examples** | Notion, Linear, Jira templates | Medium |
| **Multi-language** | Non-English knowledge base | Low |

---

## Decision Log

### Decisions Made (Original)

| Decision | Choice | Rationale |
|----------|--------|-----------|
| Agent depth | Medium | Balance context size vs capability |
| Cross-agent awareness | Neighbors only | Prevent context bloat |
| One-pager template | Single operational | Strategic doc is guidance only |
| OKR requirement | Optional | Pre-seed/seed too fast for quarterly |
| Orchestrator diagnosis | Red/Blue phase | Determines discovery vs execution focus |

### Decisions Made (December 25, 2025 Session)

| Decision | Choice | Rationale |
|----------|--------|-----------|
| Implementation platform | Simplified markdown-based | Agents are .md files Claude reads directly; no SDK needed; accessible to non-developers |
| Alignment → Stakeholder | Renamed agent | "Stakeholder" is clearer about what it does (coordination, RACI, buy-in) |
| 360 coherence check | Orchestrator owns it | Orchestrator already sees everything; checks Vision→Strategy→Roadmap→Metrics alignment |
| Deliverable question | Ask before routing | Conversations without target drift; scopes the conversation |
| Explain Red/Blue | After diagnosis | Concept not widely known; users need context to understand guidance |
| PM jokes | extra/pm-jokes.md | Add personality; make it less AI-ish; drop contextually |
| Company context | context/company-profile.md | PM work highly dependent on business context (stage, industry, geography) |
| User context | context/user-profile.md | Different users need different guidance (junior vs senior, PM vs CEO) |
| Context updates | Orchestrator suggests, user confirms | Balance automation with user control; don't auto-update without consent |
| Context building | Web search + confirm | Fast path to value; infer from website, confirm with user |
| Folder structure | Flat context/ folder | Simple, not over-engineered; uploads/ subfolder for docs |

### Decisions Pending

| Decision | Options | Blocker For |
|----------|---------|-------------|
| Multi-session persistence | File-based, external store | Long-term context retention |
| Skill triggering reliability | Description tuning, explicit invocation | Consistent skill activation |

---

## Next Steps

### Completed

1. ~~**Choose implementation platform**~~ ✓ Simplified markdown-based
2. ~~**Create proof of concept**~~ ✓ Tested with real user scenario
3. ~~**Add context system**~~ ✓ Company and user profiles

### Current Focus

1. **More real-world testing**
   - Test with different user scenarios
   - Test all agent handoffs
   - Test skill invocations

2. **Context building UX**
   - Test web search flow for company context
   - Refine onboarding experience

3. **Polish and document**
   - Ensure all CLAUDE.md files are accurate
   - Update README for first-time users

### Future (When Ready)

1. **Multi-session persistence** - How to maintain context across conversations
2. **Publishing** - GitHub release, community announcement
3. **Feedback incorporation** - Iterate based on real usage

---

## Success Criteria

### Phase 2 Complete When:
- [ ] All 7 agents have working system prompts
- [ ] All 9 utility skills are invokable
- [ ] Orchestrator can route to any agent
- [ ] Handoffs work in both directions
- [ ] Knowledge base is properly injected

### Phase 3 Complete When:
- [ ] All unit tests pass
- [ ] All integration tests pass
- [ ] All user journeys tested
- [ ] Edge cases handled gracefully
- [ ] No critical bugs

### Phase 4 Complete When:
- [ ] Prompt performance optimized
- [ ] Knowledge gaps filled
- [ ] User experience is smooth
- [ ] Feedback incorporated

### Phase 5 Complete When:
- [ ] Documentation complete
- [ ] Installation works
- [ ] GitHub release published
- [ ] Community can use it

---

## Appendix

### A. File Inventory

**Agents (7):**
```
agents/orchestrator.md
agents/vision.md
agents/strategy.md
agents/discovery.md
agents/roadmap.md
agents/metrics.md
agents/stakeholder.md
```

**Skills (11):**
```
skills/skill-creator.md
skills/prioritization.md
skills/positioning.md
skills/opportunity-tree.md
skills/okr-builder.md
skills/impact-model-builder.md
skills/metric-selector.md
skills/leading-lagging-mapper.md
skills/aarrr-analyzer.md
skills/initiative-alignment-doc.md
skills/interview-summary.md
```

**Knowledge (38):**
```
knowledge/strategy/ (7 files)
knowledge/discovery/ (9 files)
knowledge/roadmap/ (5 files)
knowledge/metrics/ (5 files)
knowledge/alignment/ (10 files)
knowledge/prioritization/ (2 files)
```

**Context (3):**
```
context/CLAUDE.md
context/company-profile.md
context/user-profile.md
context/uploads/
```

**Extra (1):**
```
extra/pm-jokes.md
```

**CLAUDE.md Files (5):**
```
CLAUDE.md (root)
agents/CLAUDE.md
skills/CLAUDE.md
knowledge/CLAUDE.md
context/CLAUDE.md
```

### B. Agent Neighbor Map

| Agent | Neighbors |
|-------|-----------|
| Orchestrator | All (+ owns context & coherence) |
| Vision | Strategy, Stakeholder |
| Strategy | Vision, Discovery, Metrics |
| Discovery | Strategy, Roadmap, Metrics |
| Roadmap | Discovery, Stakeholder, Metrics |
| Metrics | Strategy, Discovery, Roadmap |
| Stakeholder | Roadmap, Strategy, Metrics |

### C. Utility Invocation Map

| Utility | Invoked By | Mode |
|---------|------------|------|
| skill-creator | Meta | Template |
| Prioritization | User, Strategy, Roadmap | Hybrid |
| Positioning | User, Strategy | Hybrid |
| Opportunity-tree | Discovery | Agent-called |
| OKR-builder | Metrics | Agent-called |
| Impact-model-builder | Metrics | Agent-called |
| Metric-selector | Metrics | Agent-called |
| Leading-lagging-mapper | Metrics | Agent-called |
| AARRR-analyzer | Metrics | Agent-called |
| Initiative-alignment-doc | Roadmap, Stakeholder, Discovery, Strategy | Agent-called |
| Interview-summary | Discovery | Agent-called |

### D. Orchestrator Flow

```
User starts conversation
    │
    ├── 1. Check context/company-profile.md and context/user-profile.md
    │       └── If missing: Offer to build (web search + questions)
    │
    ├── 2. Diagnose Red/Blue phase
    │       └── Ask diagnostic questions (one at a time)
    │       └── Explain the phase after diagnosis
    │
    ├── 3. Check product coherence (360 view)
    │       └── Vision → Strategy → Roadmap → Metrics aligned?
    │
    ├── 4. Ask for deliverable
    │       └── "What do you want to walk away with?"
    │
    ├── 5. Route to appropriate agent
    │       └── Load agents/[agent].md
    │
    ├── 6. Operate within agent context
    │       └── Use frameworks, knowledge refs, skills
    │
    ├── 7. Suggest handoffs when needed
    │       └── Switch to new agent context
    │
    └── 8. Offer to update context profiles
            └── "I learned X, want me to add that?"
```

---

**End of Plan**
