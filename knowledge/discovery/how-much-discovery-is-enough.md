# How Much Discovery is Enough?

**Author:** Ed Biden (Hustle Badger)  
*ex Depop, JobandTalent, Rocket Internet*

---

## What Do Product Managers Do?

A solid, if rather dry answer:

> "Product managers de-risk investments in technology."

---

## Product Teams Are Expensive

When a company has a product team, it's making an investment in technology. Product teams are expensive, so that's usually a big investment.

**Typical cost of a product team:**

| Factor | Value |
|--------|-------|
| Size of team | 8 |
| Average salary | £85,000 |
| National insurance / tax | 20% |
| Office + equipment costs (monthly) | £500 |
| **Annual cost of team** | **£864,000** |
| Monthly cost of team | £72,000 |
| Weekly cost of team | £16,615 |
| Daily cost of team | £3,323 |

This is a risky investment. Results from building products are far from certain, and the team needs to be paid regardless of what happens.

---

## Product Managers Ensure a Return on Investment

Product managers help ensure that the money companies spend on product teams is a good investment. That might mean:

- Creating customer value that leads to increased margins or growth
- Reducing operating costs through simplification and automation
- Increasing the effectiveness of engineering teams to deliver more of the above

**Discovery vs Delivery:**

- **Discovery:** Deciding what to build
- **Delivery:** Building it

---

## Four Types of Risk to Mitigate

*Marty Cagan's four big risks:*

| Risk Type | Question |
|-----------|----------|
| **Value** 💰 | Do customers really want this? Do they value it? |
| **Business** ⚙️ | Can the business deliver this? Does it create operational complexity? Is this legal? |
| **Technical** </> | Can we build this? Is it scalable, secure and reliable? |
| **Usability** 👤 | Can users understand this? Do they know how it works? |

Product managers are responsible for coordinating the efforts of the product team to systematically reduce these risks, focusing on the biggest risks first.

---

## Faster Is Better

Doing the hard work to reduce risk takes time. Product teams' time is expensive. So whether you are doing discovery or delivery, you want to do it as quickly and efficiently as possible.

- **Delivery:** shipping something faster is better
- **Discovery:** learning something faster is better

---

## How Much Discovery Is Enough?

There's no easy way to answer that. You can never remove uncertainty completely. Reducing risk is a curve—you can get some confidence very quickly, but it becomes increasingly difficult to increase your confidence further.

At some point the cost of doing further discovery is more costly than the risks of shipping the feature.

Where that point is varies based on:

1. Cost of development
2. Downside scenario
3. Company maturity and culture
4. Opportunity cost

---

## 1. Cost of Development

The longer development is likely to take, the more confident you want to be before committing to build.

| Project Size | Time | Confidence Required |
|--------------|------|---------------------|
| Quick fixes | <1 week | ~20% |
| Features | 2-3 weeks | ~40% |
| Big projects | >1 month | ~60%+ |

**Tip:** Convert projected time into a real £ amount. It's easy for stakeholders to think "let's just build this already" when it's 3 weeks of another team's time. When presented as a £50k investment, they want more evidence.

### What Does 30% Confidence Mean?

This is the weighting you would put against an impact estimate to account for uncertainty (the "C" in RICE prioritization).

**Example:**
- Expected impact = £100k incremental ARR
- Confidence level = 30%
- Risk weighted impact = £30k incremental ARR

---

## 2. Downside Scenario

| Option | Feature | Downside |
|--------|---------|----------|
| A | Add new filter to search | Very limited |
| B | Add new screen to onboarding flow | Significant |
| C | Add freemium plan | Critical |

You want higher confidence for features where there's a significant downside, regardless of build time.

**Questions to assess downside:**

- Does it touch critical flows (checkout, sign up, onboarding)?
- How reversible is this feature? Can we roll it back?
- How much does it change the user experience?
- If we're wrong about our biggest assumption, what would happen?

---

## 3. Company Maturity, Scale and Culture

Different companies have different standards for "enough" discovery:

- **Scaled businesses** have much more revenue at stake if things go wrong
- **Mature businesses** have greater capability to do discovery (more research and analytical tools)

| Company Type | Confidence Zone |
|--------------|-----------------|
| Startup | 40-60% |
| Enterprise | 80-95% |

Cultural norms also matter: Booking.com likes to AB test everything. Basecamp relies heavily on intuition. Both are great businesses.

---

## 4. Opportunity Cost

| Team | Backlog | Opportunity Cost |
|------|---------|------------------|
| Team A | Bug fixing, ad hoc requests, incremental improvements | Low |
| Team B | Major strategic project | High |

Team B would want to be much more confident in a new idea before switching tasks than Team A, because the opportunity cost is higher.

---

## Assessing Risk and Confidence

Two techniques can help:

1. **Confidence Scale** – assess your confidence on a graded scale
2. **Risk Accounting** – balance the risks and confidence, decide next steps

---

## Confidence Scale

*Adapted from Itamar Gilad's confidence meter*

| Level | Confidence | Evidence |
|-------|------------|----------|
| **Intuition** | 1% | Gut feel, 1-2 sales requests |
| **Planning** | 3% | Impact model, technical spike/plan, team buy-in |
| **Anecdotal** | 10% | 3+ sales requests, 5+ customer interviews, 1+ competitor has it |
| **Research** | 30% | 5+ sales requests, 20+ customer interviews, market survey, 3+ competitors have it |
| **Data** | 95% | Behavioural analysis, fake door/Wizard of Oz test, AB testing, alpha/beta testing |

Certainty is capped at 95% because you can never be 100% sure of anything.

---

## Risk Accounting Framework

### 1. Pick Target Confidence

Consider:
- Expected effort to build
- Opportunity cost
- Potential downsides
- Outstanding risks (value, business, technical, usability)

Pick a point on the confidence scale to aim for.

### 2. Assess Current Confidence

Grade your evidence:
- **Plans:** Impact model, technical assessment, project plan
- **Qualitative:** Customer requests, user interviews, survey results
- **Quantitative:** Behavioral analysis, AB tests, limited releases

### 3. Compare Target and Current Confidence

- **Current ≥ Target:** Move to delivery
- **Current < Target:** Do more discovery

### 4. Capture Next Steps

If more discovery is needed:
- Look at the risks you've got
- Identify activities that would boost confidence
- Decide on 2-3 things to do in the following week
- Review regularly (weekly or fortnightly)

---

## Building to Learn

Sometimes shipping something *is* discovery. You might run a closed alpha test or launch an MVP to learn.

If building an MVP primarily to learn:
- Downsides are lower (fewer users affected)
- Cost of development should be lower (less concern about scalability/reliability)

Generally, invest in quick, low effort discovery activities (impact modeling, speaking to 5 customers) to justify investing in higher effort activities (customer survey, AB testing, closed testing).

---

## Common Challenges

### Discovery Is Politics

Pressures that impact discovery:
- Hitting short term metrics
- Down-time of engineering
- Showing you're delivering (something, even if wrong)
- Marketing releases
- First mover advantage

**Tips:**

**"We've reached target confidence, but stakeholders still aren't convinced"**  
They probably think the company should head in a different direction. Escalate to senior leadership for clear confirmation of strategy.

**"I'd love to do more discovery, but my engineers need work!"**  
Options:
- Discuss with tech lead whether they can take on things you're doing
- Include engineers in discovery (technical spikes, user interviews)
- Engineers work on technical debt
- Discuss with manager about resourcing

**"Does discovery always have to be a big project?"**  
Absolutely not. Run continuous discovery for a steady stream of insights rather than commissioning big research projects.

**"I'm at a startup, we don't have time/resources for discovery"**  
Discovery can be as simple as pulling together an impact model or speaking to a handful of customers. At startups, things are usually faster to build and lower risk.

**"I can't think of a way to de-risk my big bet"**  
Not all risks can be removed by discovery. Bigger bets are more visionary. It's often about understanding potential upside and downside, and taking a call at senior level about whether this is the right bet now.

---

## Worked Examples

### Example 1: Incremental Feature (Large Consumer Business)

**Scenario:** Working at Etsy-like business on incremental improvements to core experience.

| Aspect | Value |
|--------|-------|
| Target confidence | Data - 95% |
| Current confidence | Anecdotal - 10% |
| Expected effort | ~£50k (weeks) |
| Downside | None / very low |

**Next steps:**
- Quant analysis: how many users already search for colours?
- Tech spike: can we detect colour of item using ML?
- Qual analysis: prototype usability testing

### Example 2: Customer Request (B2B Company)

**Scenario:** Biggest client asking for user roles and permissions, threatening not to renew.

| Aspect | Value |
|--------|-------|
| Target confidence | Research - 30% |
| Current confidence | Intuition - 1% |
| Expected effort | ~£50k (weeks) |
| Downside | Low |

**Next steps:**
- Technical spike to see if possible
- Impact model to understand revenue potential
- Get sales team to speak to 10-20 other customers

### Example 3: Big Bet (Pre-Series A SaaS)

**Scenario:** CEO wants to validate and build freemium pricing model.

| Aspect | Value |
|--------|-------|
| Target confidence | Data - 95% |
| Current confidence | Planning - 3% |
| Expected effort | ~£250k (months) |
| Downside | Huge—could sink the business |

**Next steps:**
- Speak to 3x expert investors/advisors with freemium experience
- Interview 10+ clients on willingness to pay
- Launch waitlist to gauge demand before building

---

## Recap

Product managers are responsible for creating business value and solving customer problems. One of the most important things PMs do is manage risks by doing robust discovery.

How much discovery you need depends on:

1. How expensive it will be to build
2. What could go wrong
3. How mature your company is, and its decision-making culture
4. What else you could be building

**The Confidence Scale** allows you to grade how much you've de-risked the idea.

**Risk Accounting** helps you consider all costs and risks to decide how much discovery is enough, then focus efforts on reaching that confidence level quickly.

---

## Resources

- [Discovery Template (Google Sheets)](https://docs.google.com/spreadsheets)
- How to Build Continuous Discovery Habits
- What do Product teams do?
- Design thinking
- Customer journey map Template
- Jobs to be done Template
- Ideation Session Template

## Further Reading

- Reducing Product Risk and Removing the MVP Mindset – Casey Winters
- Doing Discovery Well: How to Measure and Guide Your Team – Teresa Torres
- The Evolution of Modern Product Discovery – Teresa Torres
- Product Discovery | A Practical Guide for Product Teams – Tim Herbig
- How much product discovery is enough – Itamar Gilad

---

*Thanks to Louise Baldwin, Nils Stotz and Joshua Sandhu for reviewing early drafts of this article.*
