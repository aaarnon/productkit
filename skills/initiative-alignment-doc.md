---
name: initiative-alignment-doc
description: Creates Product Alignment Documents for initiatives. Documents problem definition, solution, launch readiness, and impact assessment with RACI and risk frameworks. Use when documenting initiatives, creating alignment docs, preparing for stakeholder review, or recording product decisions.
---

# Initiative-Alignment-Doc Utility

## Purpose

Creates Product Alignment Documents for initiatives with problem, solution, launch, and impact sections.

---

## Invocation

**Agent-called:** Called by Roadmap, Alignment, Discovery, or Strategy agents

---

## Knowledge Folder

**Primary folder:** `knowledge/alignment/`

Search for "alignment" or "one-pager" in this folder for template guidance and the Product Operating Model. New files added to this folder are automatically available.

---

## When to Use

- Documenting a new initiative for alignment
- Creating "bet artifacts" for roadmap items
- Preparing for stakeholder review
- Recording decisions and rationale

---

## Template Structure

The Product Alignment Document has **4 sections** that evolve over the initiative lifecycle:

### Section 1: Problem Definition
*Complete during discovery/framing*

| Element | Purpose |
|---------|---------|
| **Objective** | What we're trying to achieve, company goals connection |
| **Success Metric** | How we'll measure success |
| **Stakeholders (RACI)** | Who's responsible, accountable, consulted, informed |
| **Context** | Why this matters (user + business perspective) |
| **Scope** | Now vs Later boundaries |
| **Risks** | Value, Usability, Feasibility, Business Viability |

### Section 2: Solution Definition
*Complete during design/planning*

| Element | Purpose |
|---------|---------|
| **User Flow Diagram** | Visual of user journey |
| **User Story** | Detailed workflow steps |
| **Designs** | Wireframes/mockups |
| **User Feedback** | Validation insights |
| **Decision Log** | Key decisions and rationale |

### Section 3: Launch Readiness
*Complete before launch*

| Element | Purpose |
|---------|---------|
| **Testing Plan** | Unit, integration, UAT |
| **GTM Plan** | Positioning, entry, pricing |
| **Customer Success** | Support, docs, training |
| **Compliance** | Legal, privacy, security |
| **FAQs** | Internal and external |
| **Timeline** | Milestones and checkpoints |

### Section 4: Release Impact
*Complete post-launch*

| Element | Purpose |
|---------|---------|
| **Success Metrics** | Actual results vs targets |
| **Quantitative Analysis** | Usage data, engagement |
| **Qualitative Analysis** | User feedback, testimonials |
| **Next Steps** | Follow-up actions |

---

## RACI Framework

| Role | Responsibility |
|------|----------------|
| **Responsible** | Doing the work (coding, design) |
| **Accountable** | Final decision authority |
| **Consulted** | Input before decisions |
| **Informed** | Kept up to date |

---

## Four Risks Assessment

| Risk | Question | Mitigation Approach |
|------|----------|---------------------|
| **Value** | Will customers want this? | User research, validation |
| **Usability** | Can they figure it out? | Prototyping, testing |
| **Feasibility** | Can we build it? | Technical spikes, estimates |
| **Business Viability** | Does it work for business? | Financial analysis |

---

## Output Format

```
# [Initiative Name] - Product Alignment Document

> [One-line description of what this enables for users]

## 1. Problem Definition

### Objective
[What we're trying to achieve]

### Success Metric
[Primary metric for measuring success]

### Stakeholders
| Role | Person |
|------|--------|
| Responsible | |
| Accountable | |
| Consulted | |
| Informed | |

### Context
[Why this matters - user and business perspective]

### Scope
**Now:** [Current scope]
**Later:** [Future scope]

### Risks
| Risk | Description | Mitigation |
|------|-------------|------------|
| Value | | |
| Usability | | |
| Feasibility | | |
| Business Viability | | |

---

## 2. Solution Definition
[To be completed during design]

## 3. Launch Readiness
[To be completed before launch]

## 4. Release Impact
[To be completed post-launch]
```

---

## Deeper Guidance

For understanding the 3-phase evolution (Opportunity Framing → Solution Framing → Expected Outcome), search `knowledge/alignment/` for "product alignment" or "how to use".
