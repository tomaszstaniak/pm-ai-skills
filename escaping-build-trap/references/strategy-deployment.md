# Strategy Deployment

Melissa Perri's strategy deployment framework connects high-level company vision to the daily work of product teams through a four-level cascade. Each level translates strategic direction into progressively concrete actions. When this cascade works, every team knows why their work matters and how it connects to the company's direction. When it breaks, teams either build the wrong things or build the right things for the wrong reasons.

## The Vision-to-Options Cascade

```
Company Vision (aspirational, 5+ years)
    └── Strategic Intents (company-level challenges, 2-5 years)
            └── Product Initiatives (quarterly problems to solve)
                    └── Options (weekly experiments and solutions)
```

Each level answers a different question:

| Level | Question It Answers | Time Horizon | Who Owns It | How Often It Changes |
|-------|---------------------|--------------|-------------|---------------------|
| Company Vision | Where are we going? | 5+ years | CEO / Founders | Rarely (years) |
| Strategic Intents | What challenges must we overcome to get there? | 2-5 years | Executive team | Annually |
| Product Initiatives | What problems should teams solve this quarter? | Quarterly | Product leadership | Quarterly |
| Options | What can we try this week to make progress? | Weekly | Product teams | Continuously |

## How to Write Each Level

### Level 1: Company Vision

The company vision describes the future state the company exists to create. It is aspirational, durable, and customer-centered. It does not describe the product — it describes the world the product helps create.

**Characteristics of a good vision:**
- Aspirational but believable
- Customer-centered, not company-centered
- Stable across years (if your vision changes every quarter, it is not a vision — it is a goal)
- Specific enough to guide decisions, broad enough to allow innovation
- Understandable by every employee without explanation

**Writing template:**

> We envision a world where [target customers] can [desired future state] without [current pain or limitation].

**Examples:**

| Company Type | Weak Vision | Strong Vision |
|-------------|-------------|---------------|
| B2B SaaS (HR) | "Be the leading HR platform" | "Every company, regardless of size, can build a workplace where people do their best work" |
| E-commerce | "Sell more products online" | "Every artisan can reach customers who value their craft, without needing a storefront or marketing budget" |
| Fintech | "Disrupt banking" | "Every person has access to financial tools that were previously available only to the wealthy" |
| Internal tools | "Improve operational efficiency" | "Every employee spends their time on work that requires human judgment, not on repetitive processes that software should handle" |

**Common mistakes:**
- **Too vague:** "Make the world a better place." This guides nothing.
- **Too product-specific:** "Build the best project management tool." This constrains innovation and describes a product, not a future state.
- **Company-centered:** "Become the market leader in X." This is a business goal, not a vision.
- **Unmemorable:** If employees cannot recite it from memory, it is not working as a vision.

### Level 2: Strategic Intents

Strategic intents are the major challenges the company must overcome in the next 2-5 years to make progress toward the vision. They are not projects or features — they are high-level problem statements at the company level.

**Characteristics of a good strategic intent:**
- Framed as a challenge or obstacle, not a solution
- Scoped to 2-5 years of focused effort
- Measurable at the company level (revenue, market share, customer segments served)
- Limited in number: 1-3 at any given time
- Owned by a member of the executive team

**Writing template:**

> [Challenge verb] our [specific area] so that [measurable business outcome] by [time frame].

**Examples:**

| Company Context | Weak Strategic Intent | Strong Strategic Intent |
|----------------|----------------------|----------------------|
| B2B SaaS expanding upmarket | "Build enterprise features" | "Establish credibility and product-market fit in the enterprise segment (500+ employees) to reach $20M ARR from enterprise by 2028" |
| E-commerce with retention problem | "Reduce churn" | "Transform first-time buyers into repeat customers, increasing repeat purchase rate from 15% to 40% over 3 years" |
| Platform with engagement issue | "Increase engagement" | "Make daily active usage the norm for our core user persona, moving DAU/MAU from 25% to 60% by 2027" |

**Common mistakes:**
- **Too many:** Having 7 strategic intents means having no strategic focus. If everything is strategic, nothing is.
- **Solution-disguised-as-intent:** "Build a mobile app" is a solution, not a strategic intent. The intent might be "reach customers in mobile-first markets" — the mobile app is one possible option.
- **No measurable component:** "Become more innovative" cannot be tracked. Without a measurable element, there is no way to know if you are making progress.

### Level 3: Product Initiatives

Product initiatives translate strategic intents into quarterly problems for product teams to solve. Each initiative states a specific problem, identifies who experiences it, and defines how progress will be measured. Initiatives are owned by product teams or groups of teams.

**Characteristics of a good product initiative:**
- States a problem, not a solution
- Scoped to a quarter (achievable progress in 12 weeks)
- Connected explicitly to a strategic intent
- Has a clear success metric
- Owned by a specific team

**Writing template:**

> **Initiative:** [Problem statement]
> **Connected to:** [Strategic Intent]
> **Target metric:** [Specific metric] from [current value] to [target value]
> **Owner:** [Team name]
> **Time frame:** [Quarter]

**Examples:**

| Strategic Intent | Weak Initiative | Strong Initiative |
|-----------------|----------------|-------------------|
| "Establish enterprise PMF" | "Build SSO and audit logs" | "Reduce enterprise security review rejection rate from 60% to under 15% (Q2 2026)" |
| "Transform first-time buyers into repeat customers" | "Build a loyalty program" | "Increase 90-day repeat purchase rate for first-time buyers from 15% to 22% (Q3 2026)" |
| "Make daily active usage the norm" | "Add push notifications" | "Reduce time-to-first-value for new users from 3 days to same-day (Q2 2026)" |

**Common mistakes:**
- **Feature in disguise:** "Build recommendation engine" is a solution. "Help users discover relevant products without manual searching" is a problem.
- **No baseline metric:** "Improve retention" without a current number and target number is unmeasurable.
- **Too broad for a quarter:** "Solve all onboarding problems" is too large. Pick the highest-leverage onboarding problem for this quarter.
- **Not connected to a strategic intent:** Orphan initiatives indicate strategic drift — teams working on things that do not connect to company direction.

### Level 4: Options

Options are the specific things teams can try to make progress on their initiative. They are hypotheses, experiments, and solutions — plural, because there should always be multiple options under consideration. This is where the team's creativity, expertise, and discovery work come into play.

**Characteristics of good options:**
- Framed as hypotheses with expected outcomes
- Small enough to test in 1-2 weeks
- Multiple options considered before committing to one
- Based on discovery evidence (customer research, data analysis)
- Owned by the team, not dictated by leadership

**Writing template:**

> **Option:** [Proposed solution or experiment]
> **Hypothesis:** We believe [this action] will [cause this outcome] for [these users] because [this evidence or reasoning].
> **How we will test it:** [Experiment design]
> **Success criteria:** [Metric] moves by [amount] within [time frame]

**Example set for initiative "Reduce enterprise security review rejection rate":**

| Option | Hypothesis | Test Method | Duration |
|--------|------------|-------------|----------|
| Pre-fill security questionnaire | Providing a pre-completed CAIQ reduces review time and rejection rate because 70% of rejections are due to incomplete documentation | Ship to next 10 enterprise prospects | 2 weeks |
| SOC 2 Type II certification | Having SOC 2 eliminates the most common single rejection reason (no third-party audit) | Track rejection reasons before/after | 8 weeks |
| Dedicated security review liaison | A human guide through the process reduces confusion-based rejections | Assign liaison to 5 prospects | 3 weeks |

## Alignment Workshops

### Purpose

Alignment workshops connect teams to strategy by making the cascade visible and interactive. They are not status meetings — they are sessions where teams understand the "why" behind their work and contribute to shaping the "how."

### Workshop Format: Strategy Connection Session (Half-Day)

**Attendees:** Product teams, engineering leads, design leads, product leadership. Optional: exec sponsor for the strategic intent.

**Pre-work (sent 3 days before):**
- Current company vision (1 page)
- Active strategic intents with progress updates (1-2 pages)
- Each team's current initiative and key learnings (1 page per team)

**Agenda:**

| Time | Activity | Purpose |
|------|----------|---------|
| 0:00-0:20 | Vision and strategic intents review | Ensure everyone understands the top-level direction |
| 0:20-0:50 | Each team presents: initiative, key learnings, current options | Cross-team visibility |
| 0:50-1:10 | Break | |
| 1:10-1:50 | Small group exercise: "Where are the gaps?" | Identify problems no team is working on that connect to strategic intents |
| 1:50-2:30 | Small group exercise: "Where are the conflicts?" | Identify places where team initiatives are working at cross-purposes |
| 2:30-2:45 | Break | |
| 2:45-3:15 | Full group: Prioritize gaps and conflicts | Decide what to address this quarter vs. next |
| 3:15-3:45 | Each team drafts updated initiative for next quarter | Incorporate workshop insights |
| 3:45-4:00 | Wrap-up and commitments | Capture decisions and next steps |

**Facilitation tips:**
- Use physical or digital sticky notes for the gap and conflict exercises
- Have each team present in 5 minutes or less — enforce the time limit
- The exec sponsor should listen more than talk during the first half
- Conflicts between teams are features of the workshop, not bugs — surface them early

### Workshop Format: Quick Alignment Check (90 Minutes)

Use this lighter format monthly to maintain alignment without the overhead of a half-day session.

**Agenda:**

| Time | Activity |
|------|----------|
| 0:00-0:15 | Strategic intent progress update (product leadership) |
| 0:15-0:45 | Each team: 5-minute update on initiative progress, key learnings, and blockers |
| 0:45-1:15 | Open discussion: cross-team dependencies, emerging conflicts, new information |
| 1:15-1:30 | Decisions and action items |

## Common Breakdowns in the Deployment Chain

### Breakdown 1: Missing Middle

**Symptom:** The company has a vision and teams have backlogs, but there is nothing in between. Teams cannot explain how their work connects to the vision.

**Why it happens:** Strategic intents and product initiatives require deliberate work to create and maintain. Many organizations skip them because "we all know what we are doing."

**Fix:** Run a strategy deployment workshop to create the missing levels. Start with strategic intents — ask the exec team: "What are the 2-3 biggest challenges standing between us and our vision?" Then cascade those into team-level initiatives.

### Breakdown 2: Strategy Without Options

**Symptom:** Strategic intents and initiatives exist on paper, but teams are still building predetermined feature lists. The strategy documents are shelf-ware.

**Why it happens:** Leadership creates strategy documents but then hands teams feature lists anyway. The strategy is decorative, not operational.

**Fix:** Change the handoff. Instead of giving teams solutions, give them the initiative (problem + metric). Explicitly tell teams: "Your job is to figure out the best way to move this metric. We trust you to explore options."

### Breakdown 3: Options Without Strategy

**Symptom:** Teams are experimenting and iterating, but their experiments do not connect to any strategic direction. Lots of activity, no coherent progress.

**Why it happens:** Teams embraced discovery and experimentation but were never given strategic context. They are solving problems, but not necessarily the right problems.

**Fix:** Create the strategic intents and initiatives first. Then ask teams to evaluate their current work: "Which of your current experiments connects to these initiatives? Which does not? Redirect accordingly."

### Breakdown 4: Static Cascade

**Symptom:** The cascade was created once and never updated. Strategic intents from two years ago still drive current work even though the market has changed.

**Why it happens:** Creating the cascade was treated as a one-time planning event rather than an ongoing process.

**Fix:** Institute a cadence: review strategic intents annually, review initiatives quarterly, review options weekly. The cascade is a living system, not a document.

### Breakdown 5: Cascade Without Communication

**Symptom:** The cascade exists and is maintained, but most people in the organization have never seen it or do not understand it.

**Why it happens:** Strategy deployment was treated as a leadership exercise rather than an organizational communication tool.

**Fix:** Make the cascade visible. Post it physically or digitally where teams can see it. Reference it in every planning meeting, every all-hands, every team kickoff. The strategy only works if people know what it is.

### Breakdown 6: Too Many Intents

**Symptom:** The company has 8 strategic intents, each with 5 initiatives, creating 40 simultaneous priorities. Nothing gets enough focus to make meaningful progress.

**Why it happens:** Leadership cannot say no. Every department's priority becomes a strategic intent. The cascade becomes a comprehensive list of everything the company could do rather than a focused list of what it should do.

**Fix:** Force-rank the strategic intents. Ask: "If we could only make progress on one of these this year, which one?" Then: "If we could do two?" Limit active strategic intents to 1-3 at any time. Acknowledge that the others are important but not current priorities.

## Strategy Deployment Document Template

Use this template to document and communicate your strategy cascade. Keep it to 2-3 pages maximum.

---

### [Company Name] Strategy Deployment — [Year/Quarter]

**Company Vision**
[One sentence describing the future state you are working toward]

**Strategic Intents (Active)**

**Intent 1: [Title]**
- Challenge: [What we need to overcome]
- Measure: [How we will track progress]
- Current status: [On track / Needs attention / At risk]
- Owner: [Executive name]
- Time horizon: [Target year]

**Intent 2: [Title]**
- Challenge: [What we need to overcome]
- Measure: [How we will track progress]
- Current status: [On track / Needs attention / At risk]
- Owner: [Executive name]
- Time horizon: [Target year]

**Product Initiatives ([Current Quarter])**

| Initiative | Connected Intent | Target Metric | Current → Target | Owner (Team) | Status |
|-----------|-----------------|---------------|------------------|--------------|--------|
| [Problem statement] | Intent 1 | [Metric name] | [X → Y] | [Team name] | [Status] |
| [Problem statement] | Intent 1 | [Metric name] | [X → Y] | [Team name] | [Status] |
| [Problem statement] | Intent 2 | [Metric name] | [X → Y] | [Team name] | [Status] |

**Current Options Under Exploration**

| Team | Initiative | Active Options | Status | Key Learning |
|------|-----------|---------------|--------|--------------|
| [Team] | [Initiative] | Option A: [description] | Testing | [What we have learned so far] |
| | | Option B: [description] | Planned | |
| [Team] | [Initiative] | Option C: [description] | Validated | [Evidence supporting this option] |
| | | Option D: [description] | Abandoned | [Why we stopped pursuing this] |

**Review Cadence**
- Strategic intents: Annual review ([month])
- Product initiatives: Quarterly review ([months])
- Options: Weekly team-level review
- Alignment workshop: Quarterly ([next date])

**Changes Since Last Update**
- [List any changes to intents, initiatives, or significant option decisions]

---

## Making Strategy Deployment Work

Strategy deployment fails when it is treated as a planning artifact rather than a communication and alignment tool. The document matters less than the conversations it enables. The cascade matters less than the shared understanding it creates.

Three principles for making it work:

**Principle 1: Strategy must be communicated relentlessly.** Saying it once is not enough. Reference the cascade in every planning meeting, every all-hands, every team kickoff. Leaders who think they have communicated the strategy enough have usually communicated it one-tenth as much as needed.

**Principle 2: Teams must have real autonomy at the options level.** If leadership defines the vision, intents, and initiatives but also dictates the options, the cascade is a command-and-control structure with strategic language. True strategy deployment means trusting teams to figure out how to solve the problems they have been given.

**Principle 3: Learning must flow upward.** When teams discover that an initiative is based on a wrong assumption, that learning must flow back up the cascade. If a strategic intent turns out to be less important than expected, the exec team needs to hear it and adjust. The cascade is bidirectional — strategy flows down, learning flows up.

The goal is not a perfect document. The goal is an organization where every person can answer three questions: "Where are we going?" (vision), "What stands in our way?" (strategic intents), and "What am I doing about it?" (initiatives and options). When everyone can answer those three questions, you have deployed your strategy.
