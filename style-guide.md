# Writing Style Guide

**Applies to:** Anything saved to `outputs/` (formal deliverables)
**Does NOT apply to:**
- Conversational interactions (adapt to user's tone)
- `context/` files (internal memory, not deliverables)

---

## Core Principles

1. **Keep it succinct** - No fluff. Make every word count.
2. **Minimum viable document** - What's needed to accomplish the purpose, no more. Less text is more.
3. **Executive-level focus** - Write for management discussions. If a section doesn't help make a decision, cut it.
4. **No concluding errata** - Skip "future considerations," "next steps," "benefits," or "implementation summary" sections. Flag open questions at the top, not in a conclusion.
5. **No em dashes** - Em dashes sound like AI-written text. You should sound like a human. Keep punctuation simple.

---

## Required Document Structure

All outputs must follow this structure:

### 1. Overview (Required)

2-3 sentences max. Answer:
- What is this document?
- Why does it matter now?
- What decision does it support?

### 2. Main Content

Document-specific sections.

### 3. FAQ (Recommended)

See FAQ section below for rules.

---

## Designing Documents

### Sections to Skip

Don't add sections you don't need right now. Common offenders:

| Section                      | Why to skip                             |
| ---------------------------- | --------------------------------------- |
| Stakeholder Matrix           | Only if alignment is the actual problem |
| Success Metrics (10+)        | 1-3 metrics max. More = no focus        |
| Background/Context (2 pages) | 2-3 sentences. They know the business   |

**Test:** Would a busy exec skip this section? Then cut it.

### Sections to Consider

**FAQ (Recommended)**

End documents with a short FAQ that anticipates hard questions.

**Purpose:** Surface the difficult questions an expert or skeptical exec would ask. Not softballs.

**Rules:**
- 3-5 questions max
- Strategic questions that challenge the document's assumptions or recommendations
- Prefix each answer with `[Suggested answer - Please review]` to signal these need validation
- Short answers (2-3 sentences)

**Good FAQ questions:**
- "What's the biggest risk if we're wrong about X assumption?"
- "Why not [obvious alternative]?"
- "What would make us reverse this decision?"

**Bad FAQ questions:**
- Questions already answered in main doc
- Obvious questions that don't require expertise to ask
- Setup questions designed to make the doc look good

---

## Writing Rules (Priority Order)

### 1. Omit Needless Words

Vigorous writing is concise. Make every word tell.

| Verbose | Concise |
|---------|---------|
| "the question as to whether" | "whether" |
| "owing to the fact that" | "because" |
| "in a hasty manner" | "hastily" |
| "there is no doubt but that" | "doubtless" |
| "he is a man who" | "he" |
| "at this point in time" | "now" |

**Before:** "There were a great number of dead leaves lying on the ground"
**After:** "Dead leaves covered the ground"

### 2. Use Specific, Concrete Language

Prefer specific over general, definite over vague, concrete over abstract.

| Abstract | Concrete |
|----------|----------|
| "A period of unfavorable weather set in" | "It rained every day for a week" |
| "The metric showed improvement" | "Activation rate increased from 20% to 35%" |
| "Users experienced friction" | "40% of users abandoned checkout at the payment step" |

### 3. Use Active Voice

Active voice is more direct and vigorous.

| Passive | Active |
|---------|--------|
| "The feature was shipped by the team" | "The team shipped the feature" |
| "The decision was made to prioritize X" | "We prioritized X" |
| "It was determined that..." | "We determined..." |

Use passive only when the actor is unknown or unimportant.

### 4. Put Statements in Positive Form

Make definite assertions. Avoid hesitating language.

| Negative/Weak | Positive/Strong |
|---------------|-----------------|
| "He was not very often on time" | "He usually came late" |
| "did not remember" | "forgot" |
| "did not pay attention to" | "ignored" |
| "not unlikely" | "likely" |

### 5. Place Emphasis at the End

The most important information goes at the end of the sentence.

**Weak:** "Humanity has hardly advanced in fortitude since that time, though it has advanced in many other ways"

**Strong:** "Humanity, since that time, has advanced in many other ways, but it has hardly advanced in fortitude"

---

## Document Structure

### Paragraphs

- **One paragraph per topic** - New paragraph signals new topic
- **Topic sentence first** - Reader knows the purpose immediately
- **End with consequence** - Not with digression or minor detail

### Sentences

- **Keep related words together** - Subject and verb shouldn't be separated by transferable clauses
- **Modifiers next to what they modify** - Avoid ambiguity
- **Vary structure** - Don't chain loose sentences with "and," "but," "so"
- **One tense** - Pick present or past and stick with it

### Parallel Construction

Express similar ideas in similar form.

**Inconsistent:** "Formerly, science was taught by the textbook method, while now the laboratory method is employed"

**Parallel:** "Formerly, science was taught by the textbook method; now it is taught by the laboratory method"

---

## Words to Avoid or Use Carefully

| Word | Issue | Alternative |
|------|-------|-------------|
| **Very** | Weak intensifier | Use stronger words |
| **However** | Don't start sentences with it | Place mid-sentence |
| **While** | Often misused for "and" or "but" | Use "and," "but," "although" |
| **Less/Fewer** | "Less" for quantity, "fewer" for number | "Fewer users" not "less users" |
| **Like/As** | "Like" for nouns, "as" for clauses | "Do as I say" not "do like I say" |

---

## PM Documentation Specifically

When writing PM artifacts:

1. **Lead with the problem** - Not the solution
2. **Quantify where possible** - "20% churn" not "high churn"
3. **State assumptions explicitly** - Don't hide them
4. **One recommendation** - If you have multiple, prioritize
5. **Cut the preamble** - Skip "This document outlines..." Just start.

---

## Summary

- Be direct
- Be specific
- Be concise
- Be active
- Be positive
- Put the important stuff at the end
