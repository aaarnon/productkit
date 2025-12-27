# Resources & References

Knowledge base index. Agents and skills MUST read this first to find relevant content, including cross-domain articles.

---

## How to Use This Index

### For Agents

1. **Filter by your name** in the "Used By" column
2. **Read the file** from the File column (path relative to `knowledge/`)
3. **Check cross-domain content** - An article in `strategy/` may list Discovery in "Used By"

### For Skills

1. **Filter by skill name** in the "Used By" column
2. **Read relevant files** before producing output
3. Skills are horizontal - any agent can invoke any skill, so skill-relevant articles may span multiple domains

### Examples

**Example 1: Discovery agent helping with opportunity mapping**
```
1. Filter "Used By" for "Discovery" OR "opportunity-tree"
2. Find: discovery/opportunity-solution-trees-teresa-torres.md
3. Find: discovery/prioritizing-opportunities-teresa-torres.md
4. Read both before building the opportunity tree
```

**Example 2: Strategy agent preparing OKRs**
```
1. Filter "Used By" for "Strategy" OR "okr-builder"
2. Find: metrics/okrs-product-management-herbig.md (cross-domain!)
3. Find: strategy/decisive-strategy-say-no.md
4. Read both - even though OKRs article is in metrics/, it's relevant to Strategy
```

**Example 3: User asks for impact model**
```
1. Active agent (Metrics or Roadmap) filters for "impact-model-builder"
2. Find: metrics/impact-model-roadmap-ed-biden.md
3. Read before invoking the skill
```

### Why "Used By" Combines Agents and Skills

- Agents do the reading, skills produce output
- When working toward a skill output, agent needs relevant articles
- Single column = simpler filtering, no false boundaries
- Agent names (Discovery, Strategy) and skill names (opportunity-tree, okr-builder) don't collide

---

## Vision

| Article | File | Key Concepts | Topics | Author | Used By |
|---------|------|--------------|--------|--------|---------|
| [How to Create a Product Vision](https://swkhan.medium.com/how-to-create-a-product-vision-445e1fced272) | `vision/how-to-create-product-vision-khan.md` | Vision Stack, Vision vs Mission, Vision vs Vision Statement, 6 Components Framework, Iterative Creation Process | `vision-crafting` `mission` `vision-stack` `aspirational-goals` `market-situation` | Saeed Khan | Vision, Strategy, Orchestrator, positioning, initiative-alignment-doc |
| [Crafting Compelling Product Vision](https://medium.com/@ebi_atawodi) | `vision/crafting-compelling-product-vision-atawodi.md` | Vision vs Mission, 4 Core Elements, Once Upon a Time Storytelling, Elevator Pitch, 3-Phase Process | `vision-crafting` `mission` `storytelling` `elevator-pitch` `evangelism` | Ebi Atawodi | Vision, Strategy, Stakeholder, Orchestrator, positioning, initiative-alignment-doc |

---

## Product Strategy

| Article                                                                                                         | File                                                | Key Concepts                                                                                                                                     | Topics                                                                                | Author                        | Used By                                                                                                 |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------------------- |
| [Product Strategy Frameworks](https://askgib.substack.com/p/ask-gib-a-summary-of-my-product-strategy)           | `strategy/product-strategy-gibson-biddle.md`        | DHM Model, GEM Model, GLEe Vision, SMT Framework, 8 Moats                                                                                        | `competitive-advantage` `moats` `positioning` `vision` `metrics`                      | Gibson Biddle                 | Strategy, Vision, Roadmap, Metrics, prioritization, okr-builder, metric-selector, impact-model-builder  |
| [Decisive Strategy](https://blog.ravi-mehta.com/p/great-strategy-helps-you-focus)                               | `strategy/decisive-strategy-say-no.md`              | Decisive vs Alibi Progress, Permission to Say No, Strategy-OKRs-Discovery Cycle, Specificity Cascades                                            | `decision-making` `strategic-focus` `prioritization` `OKRs`                           | Ravi Mehta, Tim Herbig        | Strategy, Orchestrator, Roadmap, Discovery, Metrics, prioritization, okr-builder, opportunity-tree      |
| [When NOT to Use Roadmap](https://www.romanpichler.com/blog/when-you-should-not-use-a-product-roadmap/)         | `strategy/when-not-to-use-roadmap-roman-pichler.md` | Roadmap Anti-Patterns, Strategy Validation Prerequisites, 3-Month Outcome Goals, Strategy Discovery Process                                      | `roadmap-readiness` `strategy-validation` `goal-setting` `early-stage`                | Roman Pichler                 | Roadmap, Strategy, Orchestrator, okr-builder, initiative-alignment-doc                                  |
| [Four Fits Growth](https://www.reforge.com/blog/four-fits-growth-framework)                                     | `strategy/four-fits-growth-framework-balfour.md`    | Four Fits Framework, PMF Isn't Enough, ARPU/CAC Spectrum, Five Ways to $100M, PMF Treadmill                                                      | `PMF` `growth` `unit-economics` `pricing` `distribution` `scaling`                    | Brian Balfour                 | Strategy, Vision, Metrics, Discovery, impact-model-builder, metric-selector, aarrr-analyzer             |
| [Four Types of Product Work](https://www.reforge.com/blog/product-work-beyond-product-market-fit)               | `strategy/four-types-product-work-reforge.md`       | Feature/Growth/Scaling/PMF Expansion Work, Feature Shadow Costs, Growth Models, "Why Us?" Test                                                   | `product-development` `growth` `scaling` `PMF` `prioritization`                       | Casey Winters, Fareed Mosavat | Strategy, Roadmap, Orchestrator, Metrics, prioritization, opportunity-tree, aarrr-analyzer              |
| [Product Market Fit](https://www.hustlebadger.com/what-do-product-teams-do/product-market-fit/)                 | `strategy/product-market-fit-hustle-badger.md`      | Three Dimensions of PMF, Five PMF Levels, 10x Better or Different, Retention Curves, Distribution as Feedback                                    | `PMF` `validation` `retention` `distribution` `pricing` `early-stage`                 | Ed Biden, Matt Walton         | Discovery, Strategy, Metrics, opportunity-tree, metric-selector, leading-lagging-mapper, aarrr-analyzer |
| [Be a Great Product Leader](https://adamnash.blog/2011/12/16/be-a-great-product-leader/)                        | `strategy/be-great-product-leader-adam-nash.md`     | Know Your Game + Keep Score, Three Responsibilities, Strategy Makes Prioritization Obvious, Force Multiplier                                     | `product-leadership` `decision-making` `prioritization` `metrics`                     | Adam Nash                     | Strategy, Orchestrator, Metrics, Roadmap, prioritization, metric-selector, okr-builder                  |
| [Going Multi-Product](https://review.firstround.com/going-multi-product-11-tactics-for-tackling-your-next-bet/) | `strategy/going-multi-product-first-round.md`       | Half-Speed Principle, 70:20:10 Resource Model, Product Completeness vs Multi-Product, Kill Underperformers                                       | `multi-product` `portfolio-strategy` `resource-allocation` `expansion`                | First Round                   | Strategy, Roadmap, Vision, prioritization, initiative-alignment-doc                                     |
| [Price Before Product](https://review.firstround.com/its-price-before-product-period/)                          | `strategy/price-before-product-first-round.md`      | WTP Discovery, Pricing Model Innovation, Four Monetization Failures, Segment-by-WTP                                                              | `pricing` `monetization` `discovery` `segmentation` `validation`                      | First Round                   | Strategy, Discovery, Metrics, interview-summary, opportunity-tree                                       |
| [Product Positioning](https://www.aprildunford.com/post/a-product-positioning-exercise)                         | `strategy/product-positioning-april-dunford.md`     | 5-Step Positioning Framework, Category Innovation, Competitive Positioning, Market Frame Strategy                                                | `positioning` `differentiation` `competitive-advantage` `market-category` `messaging` | April Dunford                 | Strategy, Vision, positioning, initiative-alignment-doc                                                 |
| Company to Product Strategy Notes                                                                               | `strategy/company-to-product-strategy-notes.md`     | Investment Thesis to Company Strategy Flow, Customer Knowledge Prerequisites, Win/Loss Analysis                                                  | `strategy-hierarchy` `customer-discovery` `vision` `validation`                       | Arnon                         | Strategy, Vision, Orchestrator, interview-summary, opportunity-tree                                     |
| Product Strategy One-Pager Template                                                                             | `strategy/product-strategy-one-pager-template.md`   | Strategy One-Pager Structure, GLEE Phasing, Value-Over-Time Visualization                                                                        | `strategy-documentation` `alignment` `stakeholder-management` `vision`                | Arnon                         | Strategy, Vision, Stakeholder, initiative-alignment-doc, positioning                                    |
| [Product Bundling](https://a16z.com/when-how-should-you-bundle-your-products/)                                  | `strategy/product-bundling-a16z.md`                 | Bundling Readiness, Discount-to-Attach-Rate Math, Segment-Specific Bundling, Revenue Cannibalization                                             | `pricing` `multi-product` `monetization` `segmentation` `B2B` `B2C`                   | a16z                          | Strategy, Metrics, metric-selector, impact-model-builder                                                |
| [B2B vs B2C Strategy](https://herbig.co/b2b-vs-b2c-product-strategy/)                                           | `strategy/b2b-vs-b2c-product-strategy-herbig.md`    | B2B vs B2C Differences, Hybrid Models, B2C-to-B2B Expansion Pattern                                                                              | `B2B` `B2C` `strategy-patterns` `decision-making` `stakeholder-management`            | Tim Herbig                    | Strategy, Vision, Orchestrator, initiative-alignment-doc, positioning                                   |
| [Product Strategy Patterns](https://herbig.co/product-strategy-patterns/)                                       | `strategy/product-strategy-patterns-herbig.md`      | Three Strategy Patterns (Strategic Narrative/Playing Field/Winning Moves), Patterns vs Templates                                                 | `strategy-patterns` `vision` `prioritization` `goal-setting`                          | Tim Herbig                    | Strategy, Vision, Orchestrator, okr-builder, initiative-alignment-doc                                   |
| [Product Strategy Choices](https://herbig.co/product-strategy-choices/)                                         | `strategy/product-strategy-choices-herbig.md`       | Explicit vs Implicit Choices, Strategy-to-OKR Translation, Generic vs Actionable Strategy                                                        | `decision-making` `prioritization` `OKRs` `strategy-execution`                        | Tim Herbig                    | Strategy, Roadmap, Metrics, prioritization, okr-builder, initiative-alignment-doc                       |
| Product Strategy Foundations                                                                                    | `strategy/product-strategy-foundations-herbig.md`   | Three Strategy Patterns, Stable Core vs Dynamic Peripherals, Four Pillars (IDEA/VALUE/CAPABILITIES/MARKET), Strategy-Metrics Sandwich, MAC Cycle | `strategy-patterns` `vision` `metrics` `OKRs` `goal-setting`                          | Tim Herbig                    | Strategy, Vision, Metrics, Roadmap, okr-builder, metric-selector, leading-lagging-mapper                |

---

## OKRs & Metrics

| Article | File | Key Concepts | Topics | Author | Used By |
|---------|------|--------------|--------|--------|---------|
| [OKRs for Product Management](https://herbig.co/okrs-product-management/) | `metrics/okrs-product-management-herbig.md` | Three OKR Attributes, Product Strategy-Metrics Sandwich, Outcome vs Output OKRs, Leading vs Lagging, Discovery OKRs | `OKR-fundamentals` `outcome-focus` `strategic-alignment` `discovery-metrics` | Tim Herbig | Metrics, Strategy, Roadmap, Discovery, Orchestrator, okr-builder, leading-lagging-mapper, metric-selector |
| [Escape OKR Theatre](https://www.antmurphy.me/newsletter/escape-okr-theatre) | `metrics/escape-okr-theatre-ant-murphy.md` | OKR Theatre Symptoms, Best Practices, Goodhart's Law, OKR Health Check | `OKR-pitfalls` `strategic-foundation` `goal-reduction` `anti-patterns` | Ant Murphy | Metrics, Strategy, Orchestrator, okr-builder, metric-selector |
| [Impact Model for Roadmap](https://www.hustlebadger.com/what-do-product-teams-do/building-an-impact-model-for-your-product-roadmap/) | `metrics/impact-model-roadmap-ed-biden.md` | 7-Step Impact Model, Driver Trees, Company vs Team Level, Auditability Practices, Cell Marking Convention | `impact-estimation` `financial-forecasting` `driver-trees` `model-building` | Ed Biden | Metrics, Roadmap, Strategy, impact-model-builder, okr-builder, prioritization |
| [Choosing Success Metrics](https://www.hustlebadger.com/metrics/success-metrics/) | `metrics/choosing-success-metrics-hustle-badger.md` | 5 Steps to Define Success Metric, 5 Lenses for Metric Design, Leading vs Lagging Trade-offs, Common Traps | `success-metric-selection` `metric-design` `leading-indicators` `funnel-analysis` | Ed Biden | Metrics, Discovery, Strategy, metric-selector, leading-lagging-mapper, aarrr-analyzer |
| [Revenue & Retention Metrics](https://www.hustlebadger.com/metrics/product-success-metrics/) | `metrics/revenue-retention-metrics-hustle-badger.md` | Cohort Analysis, Gross vs Net Churn, ARR/MRR, Net Revenue Retention, CLTV:CAC Ratio | `retention-tracking` `revenue-metrics` `profitability` `churn-analysis` `B2B` `B2C` | Susannah Belcher | Metrics, Strategy, Vision, metric-selector, leading-lagging-mapper, aarrr-analyzer |
| [Leading Product Metrics](https://www.hustlebadger.com/metrics/product-metrics/) | `metrics/leading-product-metrics-hustle-badger.md` | 71x Metrics Cheat Sheet, 6 Criteria for Good Leading Metrics, CMGR, DAU/WAU/MAU, Stickiness, Activation Metrics | `leading-indicators` `traffic-analysis` `activation` `stickiness` `vanity-metrics` | Susannah Belcher | Metrics, Discovery, Strategy, metric-selector, leading-lagging-mapper, aarrr-analyzer |

---

## Discovery & Opportunity Mapping

| Article | File | Key Concepts | Topics | Author | Used By |
|---------|------|--------------|--------|--------|---------|
| [20 Paths to PMF](https://review.firstround.com/20-lessons-from-20-different-paths-to-product-market-fit-advice-for-founders-from-founders/) | `discovery/20-lessons-pmf-first-round.md` | 5 Whys Framework, Problem vs Solution Validation, Hot Knife Test, ICP Testing, Design Partner Selection | `PMF` `validation` `ICP` `customer-conversations` `market-timing` `positioning` | First Round | Discovery, Strategy, Vision, interview-summary, positioning |
| [Measure Product-Market Fit](https://review.firstround.com/how-to-measure-product-market-fit/) | `discovery/measure-pmf-first-round.md` | Sean Ellis Survey (40%), North Star Metric, 30 Customer Conversations, MVP Strategy, Retention Curves | `PMF` `validation` `metrics` `surveys` `confidence` `north-star-metric` | First Round | Discovery, Strategy, Metrics, Orchestrator, metric-selector, leading-lagging-mapper |
| [Opportunity Solution Trees](https://www.producttalk.org/opportunity-solution-trees/) | `discovery/opportunity-solution-trees-teresa-torres.md` | OST 4-Layer Structure, Opportunity Space Mapping, Prioritization Without Effort Scoring, Experience Mapping | `opportunity-mapping` `OST` `discovery-framework` `prioritization` `assumption-testing` | Teresa Torres | Discovery, Strategy, Roadmap, opportunity-tree, prioritization, impact-model-builder |
| [Product Discovery](https://herbig.co/product-discovery/) | `discovery/product-discovery-herbig.md` | Dual-Track Agile, Problem Space vs Solution Space, Alibi-Discovery, Outcome Quadrant, Impact-Uncertainty Matrix | `discovery-framework` `dual-track-agile` `problem-space` `impact-mapping` `OKRs` | Tim Herbig | Discovery, Strategy, Roadmap, Orchestrator, impact-model-builder, okr-builder, opportunity-tree, prioritization |
| [How Much Discovery](https://www.hustlebadger.com/what-do-product-teams-do/how-to-write-a-great-product-strategy/) | `discovery/how-much-discovery-is-enough.md` | Four Risks, Confidence Scale (1%-95%), Risk Accounting Framework, Discovery as De-Risking Investment | `confidence` `risk-management` `discovery-scope` `validation-depth` `cost-benefit` | Ed Biden | Discovery, Strategy, Orchestrator, Roadmap, prioritization, impact-model-builder |
| [Prioritizing Opportunities](https://www.producttalk.org/prioritize-opportunities/) | `discovery/prioritizing-opportunities-teresa-torres.md` | Opportunity-First Prioritization, Hierarchical Tree Structure, Two-Way Door Decisions, Customer Language Framing | `prioritization` `opportunity-mapping` `decision-making` `opportunity-tree` | Teresa Torres | Discovery, Strategy, Roadmap, opportunity-tree, prioritization |
| [Story-Based Interviews](https://www.producttalk.org/customer-interviews/) | `discovery/story-based-interviews-teresa-torres.md` | Story-Based Interviewing, Specific Past Events, Cognitive Bias Counteraction, Pattern Recognition | `user-research` `interviews` `validation` `qualitative-research` `bias-mitigation` | Teresa Torres | Discovery, Strategy, interview-summary |
| [Continuous Interviewing](https://www.producttalk.org/continuous-interviewing/) | `discovery/continuous-interviewing-teresa-torres.md` | Continuous Interviewing, Keystone Habit, Weekly Cadence, Automated Recruitment, Deliberate Practice | `interviews` `user-research` `continuous-discovery` `habit-building` | Teresa Torres | Discovery, interview-summary |
| [Interview Snapshot](https://www.producttalk.org/2022/06/interview-snapshot/) | `discovery/interview-snapshot-teresa-torres.md` | Interview Snapshots, One-Page Synthesis, Experience Mapping, Opportunities vs Insights, Memorable Quotes | `interviews` `synthesis` `interview-snapshots` `pattern-recognition` `documentation` | Teresa Torres | Discovery, interview-summary |
| [No Time for Discovery](https://www.producttalk.org/no-time-for-discovery/) | `discovery/no-time-for-discovery-teresa-torres.md` | Minimum Viable Discovery, 7 Obstacles, Async Stakeholder Management, Discovery as Risk Reduction | `discovery-practice` `time-management` `risk-reduction` `organizational-buy-in` | Teresa Torres | Discovery, Orchestrator, Stakeholder |
| Opportunities Backlog Workflow | `discovery/opportunities-backlog-workflow.md` | High-Level Opportunities Backlog, Definition Effort, Functionality vs Capability, Backlog/Parking Lot/Bin Triaging | `opportunity-mapping` `workflow` `prioritization` `backlog-management` `OKRs` | Arnon | Discovery, Roadmap, Strategy, Orchestrator, opportunity-tree, prioritization |

---

## Roadmapping

| Article | File | Key Concepts | Topics | Author | Used By |
|---------|------|--------------|--------|--------|---------|
| [Messy Middle](https://review.firstround.com/how-to-shape-remarkable-products-in-the-messy-middle-of-building-startups/) | `roadmap/messy-middle-first-round.md` | Time as Currency, First Mile Experience, Lazy-Vain-Selfish Principle, Do > Show > Explain, Feature Creep | `product-optimization` `user-onboarding` `first-mile` `UX-principles` | Scott Belsky | Roadmap, Discovery, Strategy, prioritization |
| [The Basics](https://cutlefish.substack.com/p/tbm-1252-the-basics) | `roadmap/the-basics-john-cutler.md` | Eight Basics, Bet One-Pagers, Learning Backlog, Last Responsible Moment, Persistent Input Metrics | `minimal-viable-process` `team-fundamentals` `bet-management` `learning-reviews` | John Cutler | Roadmap, Metrics, Discovery, Orchestrator, okr-builder, metric-selector, leading-lagging-mapper |
| [Roadmap Templates](https://www.hustlebadger.com/what-do-product-teams-do/product-roadmap-templates/) | `roadmap/product-roadmap-templates.md` | 6 Roadmap Templates, Red vs Blue Phases, Rocks-Pebbles-Sand Prioritization, Gantt Chart Vicious Cycle | `roadmap-formats` `stakeholder-communication` `planning-levels` `resource-allocation` | Ed Biden | Roadmap, Orchestrator, Strategy, Stakeholder, prioritization, initiative-alignment-doc |
| [Strategic Roadmap Pt 1](https://swkhan.medium.com/how-to-create-a-real-strategic-roadmap-part-1-4916926f39b5) + [Pt 2](https://swkhan.medium.com/how-to-create-a-real-strategic-roadmap-part-2-81ba376a5d38) | `roadmap/strategic-roadmap-saeed-khan.md` | Vision Stack, SMT Objectives, Roger Martin's Strategy Definition, Business vs Product Roadmaps | `strategic-planning` `objectives-setting` `vision-alignment` `HMW-questions` | Saeed Khan | Strategy, Roadmap, Vision, Orchestrator, opportunity-tree, okr-builder |
| [Roadmap Dates](https://www.romanpichler.com/blog/should-product-roadmaps-have-dates/) | `roadmap/roadmap-dates-roman-pichler.md` | Outcome-Based Roadmaps, Iron Triangle, Now-Next-Later Framework, External vs Internal Roadmaps | `roadmap-timing` `stakeholder-management` `trade-offs` `roadmap-audiences` | Roman Pichler | Roadmap, Stakeholder, Orchestrator, initiative-alignment-doc |
| [Mission to Vision to Strategy to Roadmap](https://www.lennysnewsletter.com/p/mission-vision-strategy-goals-roadmap) | `roadmap/mission-vision-strategy-goals-roadmap-lenny.md` | Strategic Pyramid, Opportunity Solution Tree, Strategy as 3-5 Investments, Sequential Strategy Execution | `strategic-hierarchy` `vision-crafting` `mission-definition` `goal-setting` | Lenny Rachitsky | Vision, Strategy, Roadmap, Orchestrator, okr-builder, opportunity-tree, positioning |
| [Three Feature Buckets](https://adamnash.blog/2009/07/22/guide-to-product-planning-three-feature-buckets/) | `roadmap/three-feature-buckets-adam-nash.md` | Three Buckets (Metrics Movers/Customer Requests/Customer Delight), 40/30/30 Allocation, Intellectual Honesty | `feature-categorization` `resource-allocation` `prioritization-balance` `team-health` | Adam Nash | Roadmap, Strategy, Metrics, prioritization, initiative-alignment-doc |
| [5 Steps Features to Outcome](https://www.antmurphy.me/newsletter/5-steps-from-features-to-outcome-roadmap) | `roadmap/features-to-outcome-roadmap-ant-murphy.md` | 5-Step Transformation, Narrative Extraction, Now-Next-Later Prioritization, Narrative-Driven Roadmapping | `roadmap-transformation` `strategic-narrative` `feature-organization` `outcome-definition` | Ant Murphy | Roadmap, Strategy, Orchestrator, prioritization, initiative-alignment-doc, okr-builder |

---

## Prioritization

| Article | File | Key Concepts | Topics | Author | Used By |
|---------|------|--------------|--------|--------|---------|
| [VEUC Framework](https://www.antmurphy.me/newsletter/is-urgency-the-missing-ingredient-in-prioritisation) | `prioritization/veuc-prioritization-framework.md` | VEUC (Value/Effort/Urgency/Confidence), Urgency as Explicit Dimension, Time-Sensitivity, 1-3 Scoring | `prioritization-scoring` `urgency` `time-sensitivity` `stakeholder-alignment` | Ant Murphy | Orchestrator, Roadmap, Stakeholder, Discovery, prioritization, initiative-alignment-doc |
| [High Velocity Decisions](https://www.hustlebadger.com/what-do-product-teams-do/high-velocity-decision-making/) | `prioritization/high-velocity-decision-making.md` | Type 1 vs Type 2 Decisions, 80/20 Information Gathering, Benefits-Costs-Mitigations Framework, Disagree and Commit | `decision-making` `speed` `risk-management` `reversibility` `consensus-vs-velocity` | Ed Biden | Orchestrator, Strategy, Discovery, Roadmap, Stakeholder, prioritization, opportunity-tree, okr-builder |
| [Can Do vs Should Do](https://cutlefish.substack.com/p/tbm-1652-can-do-vs-should-do) | `prioritization/can-do-vs-should-do-cutler.md` | 9-Box Matrix, Box 1 = Blocked Strategic Work, Organizational vs Technical Difficulty, Unblocking as Real Work | `feasibility` `strategic-blockers` `organizational-dysfunction` `dependencies` | John Cutler | Orchestrator, Strategy, Roadmap, Stakeholder, prioritization, opportunity-tree, initiative-alignment-doc |
| Prioritization Strategy | `prioritization/prioritization-strategy.md` | "Priority Should Be Obvious", Logarithmic Results Distribution, DHM Assessment, Four Work Types by Stage, Focus Test | `strategy-clarity` `focus` `logarithmic-impact` `work-types` `company-stage` | Arnon | Orchestrator, Strategy, Discovery, Roadmap, Stakeholder, prioritization, positioning, opportunity-tree, impact-model-builder |
| RICE Framework Critique | `prioritization/rice-framework-critique.md` | RICE Critique, Scoring = Illusion of Objectivity, Story Beats Score, Binary Risk Question | `anti-framework` `scoring-critique` `risk-tolerance` `product-judgment` | Arnon | Orchestrator, Strategy, Stakeholder, prioritization, initiative-alignment-doc |

---

## Alignment & Execution

| Article | File | Key Concepts | Topics | Author | Used By |
|---------|------|--------------|--------|--------|---------|
| [Product Team Stages](https://review.firstround.com/how-to-craft-your-product-team-at-every-stage-from-pre-product-market-fit-to-hypergrowth/) | `alignment/product-team-stages-first-round.md` | 4 Phases (Drunken Walk/PMF/Hypergrowth/Scale), PM Role Evolution, Team Structure by Phase | `company-stages` `pre-PMF` `PMF` `hypergrowth` `scale` `role-evolution` `hiring` | First Round | Orchestrator, Strategy, Stakeholder, okr-builder, prioritization |
| [Project Management for PMs](https://www.hustlebadger.com/what-do-product-teams-do/project-management-for-pms/) | `alignment/project-management-for-pms.md` | Red vs Blue Phases, 5 Pillars, MoSCoW Prioritization, War Rooms, Decision Logs, RAG Status | `red-phases` `blue-phases` `project-management` `delivery` `deadline-management` | Evie Brockwell | Orchestrator, Roadmap, Stakeholder, initiative-alignment-doc, okr-builder |
| [Quarterly Strategy Meeting](https://gibsonbiddle.medium.com/how-to-run-a-quarterly-product-strategy-meeting-a-board-meeting-for-product-3a14c4d53d1b) | `alignment/quarterly-product-strategy-meeting-biddle.md` | Quarterly Strategy Meeting Structure, DHM Model, GLEe Model, SMT Alignment, Swim Lanes, 75/25 Balance | `quarterly-planning` `strategy-communication` `DHM` `swim-lanes` `results-culture` | Gibson Biddle | Strategy, Metrics, Stakeholder, Orchestrator, okr-builder, impact-model-builder, initiative-alignment-doc |
| [Data-Informed Cycle](https://cutlefish.substack.com/p/tbm-852-the-data-informed-product) | `alignment/data-informed-product-cycle-cutler.md` | 6-Stage Loop (Strategy/Models/Metrics/Leverage Points/Bets/Learning), Messy Middle, North Star Framework | `data-informed` `strategy-to-execution` `mental-models` `leverage-points` `learning-loops` | John Cutler | Strategy, Metrics, Discovery, Roadmap, impact-model-builder, metric-selector, leading-lagging-mapper, aarrr-analyzer |
| [Product Operating Model](https://www.producttalk.org/the-product-operating-model/) | `alignment/product-operating-model-teresa-torres.md` | 3 Principles (Outcome Focus/Continuous Discovery/Cross-Functional), Product Trios, Pilot Team Approach | `operating-model` `continuous-discovery` `outcome-focus` `product-trios` `transformation` | Teresa Torres | Orchestrator, Discovery, Stakeholder, Strategy, interview-summary, okr-builder, initiative-alignment-doc |
| [Business Impact to Roadmap](https://www.justanotherpm.com/blog/how-to-translate-business-impact-to-a-product-roadmap) | `alignment/translate-business-impact-to-roadmap-arora.md` | 4-Level Framework, Top-Down/Bottom-Up Flows, Limited Universe, Problem Sequencing, Impact Translation | `business-product-alignment` `impact-translation` `problem-sequencing` `portfolio-thinking` | Sid Arora | Strategy, Roadmap, Metrics, Orchestrator, okr-builder, impact-model-builder, leading-lagging-mapper, initiative-alignment-doc |
| Six Steps Production Process | `alignment/six-steps-production-process.md` | 6 Stages (Objective/Problems/Ideation/Exploration/Delivery/Follow-up), Cyclical Feedback, One-Pagers | `product-lifecycle` `process` `stage-gates` `feedback-loops` `problem-definition` | Hustle Badger | Orchestrator, Discovery, Roadmap, Metrics, opportunity-tree, okr-builder, initiative-alignment-doc |
| Product Alignment Document Template | `alignment/product-alignment-document-template.md` | 4-Section Template, RACI Matrix, Four Risk Types, User Flows, Decision Log, Launch Readiness | `alignment-template` `RACI` `risk-types` `user-flows` `launch-readiness` | Arnon | Discovery, Roadmap, Stakeholder, Metrics, initiative-alignment-doc, impact-model-builder |
| How to Use Product Alignment Doc | `alignment/how-to-use-product-alignment-doc.md` | 3 Phases (Opportunity/Solution/Expected Outcome), Problem Statement, Dependencies, GTM, 4 Decision Outcomes | `alignment-documents` `problem-framing` `solution-framing` `dependencies` `GTM` | Arnon | Discovery, Roadmap, Stakeholder, Strategy, initiative-alignment-doc, opportunity-tree, okr-builder |
| [Break Frameworks](https://www.antmurphy.me/newsletter/dont-follow-frameworks-break-them) | `alignment/break-frameworks-ant-murphy.md` | Frameworks = Tools Not Blueprints, Lattice Approach, 4 Maturity Levels, 5 Pre-Use Questions | `meta-frameworks` `adaptation` `context-sensitivity` `mastery-levels` | Ant Murphy | All agents, All skills |
| [Great One Pagers](https://publish.obsidian.md/cutlefish/Great+One+Pagers) | `alignment/great-one-pagers-john-cutler.md` | Bet Thought Exercise, 10 Qualities of Great One-Pagers, Problems > Solutions, 40 Workshop Questions, Behavioral Change Model | `one-pagers` `bets` `risk` `opportunity-sizing` `behavioral-change` | John Cutler | Roadmap, Discovery, Stakeholder, Strategy, initiative-alignment-doc, opportunity-tree, impact-model-builder |
| [PM is Business Management](https://swkhan.medium.com/product-management-is-business-management-why-does-everyone-forget-that-85f777da30e1) | `alignment/product-management-is-business-management.md` | 4 Key Principles, 5 Dysfunctions, McElroy Memo (1931), Sales = THIS Year, Product = NEXT Year | `business-management` `PM-role-definition` `business-objectives` `leading-lagging` | Saeed Khan | Orchestrator, Strategy, Metrics, okr-builder, impact-model-builder, leading-lagging-mapper |

---

## Project Inspirations

| Project | What to Learn |
|---------|---------------|
| [Ideation Agent](https://github.com/Elsevanderberg1/ideation-agent) | 7-phase workflow, CLI interview approach |
| [From Thinking to Coding](https://github.com/talsraviv/from-thinking-to-coding) | 5-phase approach, conversational interviewing |
| [BMAD Method](https://github.com/bmadcode/BMAD-METHOD) | Multi-agent architecture, 21 agents, 4 modules |

---

## Key Authors

| Author | Expertise | Website |
|--------|-----------|---------|
| Adam Nash | Product Planning, Feature Buckets, Know Your Game | adamnash.blog |
| Ant Murphy | Roadmapping, OKRs, Prioritization, Framework Adaptation | antmurphy.me |
| April Dunford | Product Positioning | aprildunford.com |
| Brian Balfour | Growth Strategy, Four Fits | reforge.com |
| Casey Winters | Growth, PMF Expansion | reforge.com |
| Ebi Atawodi | Product Vision, Leadership | ex-Uber, YouTube, Netflix |
| Ed Biden | Discovery, Risk Management, Impact Models | hustlebadger.com |
| Evie Brockwell | Project Management, Execution | hustlebadger.com |
| Fareed Mosavat | Product-Led Growth, Experimentation | reforge.com |
| Gibson Biddle | Product Strategy, DHM, GLEe | gibsonbiddle.medium.com |
| John Cutler | Product Thinking, Roadmaps, One-Pagers | cutlefish.substack.com |
| Lenny Rachitsky | Product Strategy, Growth | lennysnewsletter.com |
| Ravi Mehta | Product Strategy | ravi-mehta.com |
| Roman Pichler | Product Roadmaps, Agile | romanpichler.com |
| Saeed Khan | Strategic Roadmaps, PM as Business Management | swkhan.medium.com |
| Sid Arora | Impact Translation | justanotherpm.com |
| Susannah Belcher | Metrics | hustlebadger.com |
| Teresa Torres | Product Discovery, OST, Continuous Interviewing | producttalk.org |
| Tim Herbig | Product Discovery, OKRs, Strategy Patterns | herbig.co |

---

## Notes

- File paths are relative to `knowledge/` folder
- All files follow format in `knowledge/CLAUDE.md`
- **Used By** lists both agents and skills - filter by either
- Topics use backticks for easy scanning
