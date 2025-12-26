# Be Cautious with RICE (and Similar Scoring Frameworks)

**Author:** Arnon (with community insights)
**Type:** Personal notes

---

## The Core Problem

RICE takes 4 made-up numbers, does a calculation, and pretends the result isn't also a made-up number.

It's a "Wizard of Oz" approach - artificially inflating the credibility of a decision through the illusion of objectivity.

---

## What Actually Convinces Stakeholders

Instead of: "This feature scored 847 in RICE"

Say this:
> "We're trying to improve conversion. Analytics says our biggest funnel drop is here. Usability testing says this is the biggest problem in that step. We're fixing that first."

**Story beats score.** A clear narrative connecting data to decision is more credible than a calculated number.

---

## Why RICE Breaks Down

### 1. Absolves PMs of Real Decisions

RICE tries to remove the PM from making prioritization decisions in ambiguity. But the ambiguity doesn't disappear because you gave it a score.

### 2. Equal Weighting Kills Impact Differentiation

Because each score gets equal weight, the difference between "medium impact" and "massive impact" is only ~2 points.

But in reality:
- Massive impact initiatives rarely have high confidence
- Medium impact features often take less time

So the math often looks like:

| Feature | Impact | Confidence | Result |
|---------|--------|------------|--------|
| Massive bet | 3 pts | 25% | 0.75 |
| Medium safe | 1 pt | 100% | 1.0 |

The medium-safe feature "wins" despite being less transformational.

### 3. Drags Toward Safe Decisions

The framework systematically favors:
- Medium impact over massive impact
- Short-term over long-term
- Features stakeholders already care about
- Things less likely to fail

It penalizes the bets that could make your business way better.

---

## A Better Approach

**Eliminate the confidence score entirely.** We vastly overestimate our confidence anyway, and it creates drag on high-impact initiatives.

**Replace with a binary question:**

> "Is this risk worth taking right now?" - Pass/Fail

That's the actual decision you need to make. Force yourself to make it directly instead of hiding behind a formula.

---

## When Scoring Frameworks Can Help

Scoring isn't useless - it can help:
- Structure initial discussions
- Surface assumptions for debate
- Compare within similar-sized initiatives

But don't let the score make the decision. The score is a conversation starter, not a conclusion.

---

## So What?

1. Be skeptical of any framework that claims to remove ambiguity through math
2. Tell stories that connect data to decisions
3. If using RICE, treat it as input to discussion, not the answer
4. For high-impact bets, ask "is this risk worth taking?" directly
5. Remember: prioritization is a judgment call - own it

---

**See also:** `prioritization/prioritization-strategy.md` - "Priority should be obvious from strategy"
