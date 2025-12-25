# Skill-Creator Utility

## Purpose

Creates well-structured skills that Claude reliably discovers and triggers. Use this as the base template for writing any new skill.

---

## Why Skills Fail to Trigger

| Problem | Cause | Fix |
|---------|-------|-----|
| Skill never activates | Vague description | Be specific, include trigger terms |
| Wrong skill activates | Overlapping descriptions | Differentiate clearly |
| Partial activation | Missing context | Include "when to use" in description |
| Inconsistent behavior | Wrong point-of-view | Always use third person |

---

## SKILL.md Structure

```yaml
---
name: skill-name
description: [What it does] + [When to use it]. Include specific trigger terms.
---

# Skill Title

## Quick Start
[Minimal example to get started]

## Process
[Step-by-step instructions]

## Output Format
[Template or expected output]

## References
[Links to bundled files if needed]
```

---

## Critical Rules for Triggering

### 1. Description is Everything

The `description` field is the PRIMARY triggering mechanism. Claude uses it to decide which skill to activate.

**Good description:**
```yaml
description: Synthesizes customer interview notes into one-page summaries with quotes, experience maps, and opportunities. Use when processing interview notes, creating interview summaries, or extracting customer insights from conversations.
```

**Bad description:**
```yaml
description: Helps with interviews
```

### 2. Always Third Person

Description is injected into system prompt. Inconsistent POV breaks discovery.

| Good | Bad |
|------|-----|
| "Processes Excel files and generates reports" | "I can help you process Excel files" |
| "Creates interview summaries from notes" | "You can use this to summarize interviews" |

### 3. Naming Conventions

`name` field: lowercase, hyphens only, max 64 chars.

**Preferred (gerund form):**
- `processing-pdfs`
- `analyzing-interviews`
- `building-roadmaps`

**Acceptable (noun phrase):**
- `interview-summary`
- `opportunity-tree`

**Avoid:**
- Vague: `helper`, `utils`, `tools`
- Generic: `documents`, `data`

---

## Skill Creation Process

### Step 1: Define Usage
- What tasks should trigger this skill?
- What would a user say?
- What terms/phrases should activate it?

### Step 2: Write Description First
Before any content, write the description with:
- What the skill does (specific actions)
- When to use it (trigger contexts)
- Key terms users might say

### Step 3: Write Minimal Content
- Only add what Claude doesn't already know
- Prefer examples over explanations
- Keep SKILL.md body under 500 lines

### Step 4: Test Triggering
Ask yourself: "If I said [X], would this skill activate?"
- Test with various phrasings
- Ensure description covers all trigger scenarios

---

## Content Guidelines

### Concise is Key
Context window is shared. Every token competes with conversation history.

**Good (50 tokens):**
```markdown
## Extract text
Use pdfplumber:
\`\`\`python
import pdfplumber
with pdfplumber.open("file.pdf") as pdf:
    text = pdf.pages[0].extract_text()
\`\`\`
```

**Bad (150 tokens):**
```markdown
## Extract text
PDF files are a common format containing text and images.
To extract text, you need a library. There are many options
but we recommend pdfplumber because it's easy to use...
```

### Degrees of Freedom

| Freedom | When | Example |
|---------|------|---------|
| **High** | Multiple valid approaches | "Analyze the code structure" |
| **Medium** | Preferred pattern exists | Parameterized template |
| **Low** | Fragile/critical operations | Exact script to run |

### Progressive Disclosure

- SKILL.md = overview + navigation
- Reference files = detailed content (loaded as needed)
- Keep references one level deep

---

## Template for New Skills

```yaml
---
name: [lowercase-with-hyphens]
description: [Action verb] [what it does] for [target]. Use when [trigger 1], [trigger 2], or [trigger 3].
---

# [Skill Name]

## Purpose
[One sentence - what this skill produces]

## When to Use
- [Trigger scenario 1]
- [Trigger scenario 2]
- [Trigger scenario 3]

## Process

### Step 1: [Action]
[Instructions]

### Step 2: [Action]
[Instructions]

## Output Format

\`\`\`
[Template structure]
\`\`\`

## Examples

**Input:** [Example input]
**Output:** [Example output]

## References
- [reference-file.md](reference-file.md) - [What it contains]
```

---

## Checklist Before Finalizing

**Triggering:**
- [ ] Description includes what + when
- [ ] Description uses third person
- [ ] Key trigger terms included
- [ ] Name follows conventions

**Content:**
- [ ] Under 500 lines
- [ ] No unnecessary explanations
- [ ] Examples over descriptions
- [ ] Consistent terminology

**Structure:**
- [ ] Clear process steps
- [ ] Output format defined
- [ ] References one level deep

---

## Anti-Patterns

| Anti-Pattern | Problem | Fix |
|--------------|---------|-----|
| "When to Use" only in body | Not seen until after triggering | Put in description |
| Too many options | Confuses Claude | Provide one default |
| Vague description | Won't trigger | Be specific with terms |
| First/second person | Breaks discovery | Use third person |
| Over-explanation | Wastes tokens | Trust Claude's knowledge |
