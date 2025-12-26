# Knowledge

The knowledge base contains 55+ articles from PM thought leaders—Gibson Biddle, Teresa Torres, Brian Balfour, April Dunford, John Cutler, and others. This is the source material that agents and skills draw from.

**Key principle:** Different experts have different philosophies. This is intentional—PM work is not one-size-fits-all. Use company context to select the right approach.

---

## Folder Organization

| Folder | Purpose | Used By |
|--------|---------|---------|
| `strategy/` | Strategic frameworks, positioning, PMF | Strategy, Vision |
| `discovery/` | Problem validation, OST, interviews | Discovery |
| `roadmap/` | Planning, sequencing, narrative modes | Roadmap |
| `metrics/` | Success measurement, OKRs, impact models | Metrics |
| `alignment/` | Stakeholder coordination, operating model | Stakeholder, Orchestrator |
| `prioritization/` | Decision frameworks, VEUC, trade-offs | All agents (utility) |

---

## How Agents Find Knowledge

**Folder-based discovery (not hardcoded file lists):**

1. Each agent knows its primary folder(s)
2. When agent needs info, it searches within those folders
3. New files added to a folder are automatically discoverable
4. No need to update agent files when adding knowledge

**Example:** Strategy agent needs positioning info
```
1. Search knowledge/strategy/ for "positioning"
2. Find product-positioning-april-dunford.md
3. Read and apply relevant content
```

---

## Handling Conflicting Information

### When Sources Conflict

**Step 1: Acknowledge it**
Don't pretend there's one right answer. Different experts have different views.

**Step 2: Use context to select**

| Context | Lean Toward |
|---------|-------------|
| Pre-PMF, small team | Simpler frameworks, less process |
| Post-PMF, scaling | More structure, cross-team alignment |
| High uncertainty | Discovery-heavy approaches |
| High conviction | Execution-focused approaches |

**Step 3: Present options if genuinely conflicting**
If context doesn't resolve it:
- "There are two schools of thought here..."
- "Option A (Teresa Torres) emphasizes X. Option B (Gibson Biddle) emphasizes Y."
- "Given your context, I'd lean toward X because..."

**Step 4: Build conviction through context**
The more you know about the company/user, the more confidently you can recommend.

### Common Conflicts

| Topic | Conflict | Resolution |
|-------|----------|------------|
| OKRs | Essential vs optional | Stage-dependent. Pre-PMF skip. Series A+ consider. |
| Roadmap format | Outcome vs feature-based | Red/Blue phase. Blue = outcomes. Red = can include features. |
| Discovery depth | How much is enough? | Risk-based. High-stakes = more. Reversible = less. |
| Prioritization | Many frameworks | If priority isn't obvious, strategy is unclear. |

---

## Adding New Knowledge

1. Follow the file format below
2. Place in the appropriate folder
3. **Add to `resources.md`** — keeps the catalog complete

### File Format

Each knowledge file must include:
- Title (H1)
- Author
- Source URL
- Sections with frameworks/concepts
- Tables for structured info
- Summary with key takeaways

---

## Do Not

- Pretend there's only one right answer
- Ignore context when recommending
- Apply heavy process to early-stage companies
- Apply startup chaos to scaling companies
- Invent frameworks not in the knowledge base
