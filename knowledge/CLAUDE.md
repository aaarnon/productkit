# Knowledge

## Format

Each knowledge file must include:
- Title (H1)
- Author
- Source URL
- Sections with frameworks/concepts
- Tables for structured info
- Summary with key takeaways

## Folder Organization

| Folder | Purpose | Used By |
|--------|---------|---------|
| `strategy/` | Strategic frameworks, positioning, PMF | Strategy, Vision |
| `discovery/` | Problem validation, OST, interviews | Discovery |
| `roadmap/` | Planning, sequencing, narrative modes | Roadmap |
| `metrics/` | Success measurement, OKRs, impact models | Metrics |
| `alignment/` | Stakeholder coordination, operating model, stages | Stakeholder, Orchestrator |
| `prioritization/` | Decision frameworks, VEUC, trade-offs | All agents (utility) |

## How Agents Use Knowledge

**Folder-based discovery (not hardcoded file lists):**

1. Each agent knows its primary folder(s)
2. When agent needs info, it searches within its folders
3. New files added to a folder are automatically discoverable
4. No need to update agent files when adding knowledge

**Example:** Strategy agent needs positioning info
```
1. Search knowledge/strategy/ for "positioning"
2. Find product-positioning-april-dunford.md
3. Read and apply relevant content
```

## Handling Conflicting Information

The knowledge base has diverse authors with different philosophies. This is intentional - PM work is not one-size-fits-all.

### When Sources Conflict

**Step 1: Acknowledge the conflict**
Don't pretend there's one right answer. Different experts have different views.

**Step 2: Use context to select**
Company stage, culture, and situation determine which approach fits:

| Context | Lean Toward |
|---------|-------------|
| Pre-PMF, small team | Simpler frameworks, less process |
| Post-PMF, scaling | More structure, cross-team alignment |
| High uncertainty | Discovery-heavy approaches |
| High conviction | Execution-focused approaches |

**Step 3: Present options when genuinely conflicting**
If context doesn't resolve it, present trade-offs and let user choose:
- "There are two schools of thought here..."
- "Option A (Teresa Torres) emphasizes X. Option B (Gibson Biddle) emphasizes Y."
- "Given your context, I'd lean toward X because..."

**Step 4: Build conviction through user context**
The more you know about the company/user, the more confidently you can recommend.

### Common Conflicts & Resolution

| Topic | Conflict | Resolution |
|-------|----------|------------|
| **OKRs** | Some say essential, others say optional | Stage-dependent. Pre-PMF skip them. Series A+ consider them. |
| **Roadmap format** | Outcome vs feature-based | Red/Blue phase. Blue = outcomes. Red = can include features. |
| **Discovery depth** | How much is enough? | Risk-based. High-stakes = more discovery. Reversible = less. |
| **Prioritization** | Many frameworks (RICE, VEUC, DHM) | If priority isn't obvious, strategy is unclear. Framework is secondary. |

### Never Do

- Pretend there's only one right answer
- Ignore context when recommending
- Apply heavy process to early-stage companies
- Apply startup chaos to scaling companies

## Rules

- Always cite source and author
- Summarize, don't copy verbatim
- Use tables for frameworks
- Include practical examples
- Tag files with relevant agents and skills in the header
- **New resources must be added to `resources.md`** — keeps the catalog complete
