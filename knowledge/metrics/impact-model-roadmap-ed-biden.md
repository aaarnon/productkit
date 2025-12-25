# Building an Impact Model for Your Product Roadmap

**Author:** Ed Biden

**Source:** https://www.hustlebadger.com/what-do-product-teams-do/building-an-impact-model-for-your-product-roadmap/

---

## Overview

An impact model is a spreadsheet that helps you estimate the impact a feature or theme of work will have, and understand how different drivers create impact.

> "All models are wrong, but some are useful." – George Box

Estimating impact is a mixture of art and science—never precise, but invaluable for making better decisions about which problems are worth solving and how to solve them.

---

## What an Impact Model Does

**Does:**
- Help understand how metrics are related
- Think through how user behavior drives business impact
- Estimate size of impact product work could have
- Forecast financial impact of product work
- Compare impact of different pieces of work
- Prevent adding low-impact work to roadmap

**Does NOT:**
- Give certainty on feature success
- Precisely predict impact
- Precisely forecast financial outcomes

---

## Why Model Impact?

| Benefit | Description |
|---------|-------------|
| **Prioritize work** | Prevents obvious mistakes like working on features with no clear mechanism for changing metrics |
| **Achieve targets** | Realistic targets come from understanding what's achievable in a given timeframe |
| **Forecast the future** | Helps CEOs/CFOs with financial forecasting |
| **Justify investment** | Makes investment requests easier to approve |

> "At Captify all PMs have to estimate potential revenue impact for each epic as part of our prioritisation process." — Amelia Waddington, CPO Captify

---

## Levels of Modeling Impact

### Company Level

CPOs and CFOs discuss business finances given product team work.

**Informs decisions like:**
- Should company change size of product teams?
- Does company need to raise money?
- How much to invest in marketing different products?
- Which streams of work are most important?
- How does sequencing affect company financials?

### Team Level

Teams estimate impact of features and initiatives.

**Answers questions like:**
- Which themes of work are likely most effective?
- Which features should we work on first?
- How much impact after X period of time?

### Converting Between Levels

Product leaders often give teams product metrics (conversion, engagement, behavioral) rather than financial numbers. Then CPO/CFO convert these to financial performance.

**Example:**
- Company X: consumer subscription with free/paid tiers
- Conversion correlates with early product engagement
- Onboarding Team gets OKR: increase sessions/day for new users
- CPO/CFO convert target to financial outcome

**Benefits of abstraction:**
- Attribution is difficult—product metrics avoid external factors
- More obvious, tactical goals for teams
- Teams often more motivated by customer experience metrics

---

## 7 Steps to Create an Impact Model

### 1. Define Your Measure of Impact

Business value is whatever the business values. Impact needs a consistent definition.

**Examples:**
- Revenue
- Hours watched per month (Netflix)
- Nights booked (Airbnb)
- Customer service tickets
- Gross Merchandise Value (GMV)
- Cost to serve
- Customer satisfaction (NPS/CSAT)

**Key:** Must be consistent across everything you compare—apples to apples.

**If stakeholders can't align on a metric:**
1. Stop. No point modeling without agreement
2. Get everyone in the same room
3. Remind everyone: track many metrics, but need common measure for prioritizing
4. Escalate if needed

---

### 2. Establish the Impact Drivers

Break down impact to metrics you can influence. More breakdown = easier to influence (fewer external factors).

**Example Driver Tree:**

```
Annualized Revenue
    └── Monthly Revenue × 12
            └── Avg Basket Size × Visitors Completing Checkout
                    └── Visitor Flows × Conversion Rates
```

**Key:** Goal is NOT maximum layers. Link impact metric to leading metrics your feature will actually change.

**Tips:**
- Talk to analysts or senior stakeholders
- Use metrics people are already familiar with
- Build on previous experiments and company context

---

### 3. Define Your Time Period

Must be consistent across everything you compare.

**Example of confusion:**

| Time period | Baseline revenue |
|-------------|------------------|
| 2022 Revenue | $100,000,000 |
| Q4 2022 Annualized | $115,385,543 |
| Jan 2023 Annualized | $122,023,306 |
| Feb 2023 Annualized | $112,645,619 |

**Key:** Doesn't matter what baseline is—matters that everyone uses the same one.

---

### 4. Get Baseline Data

Fill in baseline with actual data. Always link to source or add detailed notes.

**Tips:**
- Include links to increase credibility and auditability
- Verify output resembles reality (sanity check)

---

### 5. Estimate Uplift

This is art, not science. Techniques for directional accuracy:

**Look at past impact:**
- Similar features' past performance
- Previous quarter's team impact

**Segment analysis:**
- Which user segments perform better?
- Provides benchmarks and variability context

**Invert the question:**
- What minimum impact would make this worthwhile?
- If required metrics seem crazy → reconsider priority

---

### 6. Sense Check the Output

Before sharing, verify everything looks reasonable.

- Check surprising results (9/10 times = error)
- Fix errors before others notice → builds credibility
- 1/10 genuine surprising results = real insight

Then:
- Share for feedback on assumptions
- Use numbers for prioritization

---

### 7. Follow Up Post-Launch

Compare actual impact vs. predicted. Look at:

**Mechanism:**
- Does driver tree resemble reality?
- Does increasing X actually increase Y?
- What other drivers to include next time?

**Quantity:**
- How accurate were uplift estimates?
- What signals should you have noticed?
- What would you estimate for similar features?

> Unless you follow up, you have no feedback loop and can't improve.

---

## Best Practices

### Auditability

- Always link to data sources
- Label everything fully with definitions
- Be explicit about timeframe

### Cell Marking Convention

| Type | Description | Color |
|------|-------------|-------|
| **Inputs** | Base level data to change | Yellow |
| **Calculated** | Formulas—only model owner changes | White |
| **Outputs** | Impact numbers you care about | Blue |

### Formatting

- Use blank lines, bold, italic, borders
- **Similarity:** things that look similar are perceived as related
- **Proximity:** things closer together are more related

### No Hidden Data

- Every logical step should be visible
- Don't hide columns/rows with notes
- Split complex formulas into multiple steps

---

## Managing Stakeholder Expectations

Actual impact only determined through A/B testing post-launch. Pre-launch = prediction.

**However:** Having some idea of impact is much better than none.

> Presenting roadmaps with no thought to impact will severely undermine your credibility.

Senior leaders are used to navigating uncertainty. Have thorough conversations about what they should and should not read into your model.

---

## Summary

| Step | Purpose |
|------|---------|
| 1. Define impact measure | Consistent standard for comparison |
| 2. Establish drivers | Link impact to influenceable metrics |
| 3. Define time period | Consistent baseline for all comparisons |
| 4. Get baseline data | Ground model in reality |
| 5. Estimate uplift | Directionally correct predictions |
| 6. Sense check | Catch errors before sharing |
| 7. Follow up | Create feedback loop for improvement |

### Key Takeaways

1. **Impact modeling is essential** — Prevents low-impact work from entering roadmap
2. **Two levels** — Company (financial) and Team (product metrics)
3. **Consistent definitions** — Same impact measure and time period across comparisons
4. **Driver trees** — Break impact down to influenceable metrics
5. **Art, not science** — Use past data, segments, and inverted thinking
6. **Follow up** — No feedback loop = no improvement
7. **Auditability** — Link sources, label everything, no hidden data

---

## Resources

- [Impact Model Template (Google Sheets)](https://docs.google.com/spreadsheets/d/1HOqsqjwaalqUAFFag-Y5vA3kHs8TN9-wwxOuWSsnOHM/edit#gid=983214946)
- Related: OKR Template, Product Metrics, AARRR Pirate Metrics
