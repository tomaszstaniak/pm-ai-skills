# Setting Desired Outcomes

Continuous discovery begins with a clear desired outcome. Without one, teams chase features instead of impact. This guide covers how to set product outcomes that drive meaningful progress, avoid common anti-patterns, and cascade outcomes from company strategy down to individual product teams.

## Product Outcomes vs. Business Outcomes

The distinction between product outcomes and business outcomes is the most important concept in outcome-based planning.

**Business outcomes** are the metrics that measure the health of the business itself. They are typically financial or high-level growth metrics owned by executives:

- Annual recurring revenue (ARR)
- Customer acquisition cost (CAC)
- Net revenue retention (NRR)
- Monthly active users (MAU)
- Gross margin

**Product outcomes** are the changes in customer behavior that drive business outcomes. They are owned by product teams and are directly influenceable through product decisions:

- Percentage of new users who complete onboarding within 24 hours
- Number of collaboration actions per active workspace per week
- Percentage of free trial users who invite a second team member
- Time from first login to first value-generating action

The relationship is causal: improving a product outcome should improve a business outcome. If it does not, the product outcome is wrong.

| Dimension | Business Outcome | Product Outcome |
|-----------|-----------------|-----------------|
| **Owned by** | Executives, business unit leads | Product team (PM, designer, engineers) |
| **Directly influenceable by product team?** | No | Yes |
| **Timeframe** | Quarterly or annual | Weekly or biweekly observable |
| **Examples** | Revenue, retention rate, NPS | Feature adoption, task completion rate, time-to-value |
| **Used for** | Company strategy, investor reporting | Discovery and delivery prioritization |

A product team assigned a business outcome like "increase ARR by 15%" has no clear starting point for discovery. A team assigned "increase the percentage of trial users who reach their first 'aha moment' within 3 days" knows exactly where to start interviewing and experimenting.

## The Outcome Cascade

Outcomes flow from company mission down to individual teams. Each level translates abstract strategy into concrete, actionable metrics.

### Level 1: Company Mission and Vision

The mission defines why the company exists. The vision describes the future state the company is working toward. These rarely change.

### Level 2: Business Outcomes (Annual/Quarterly)

Leadership sets 2-4 business outcomes per planning cycle. These reflect the strategic bets for the period.

Example for a B2B SaaS company:
- Increase net revenue retention from 105% to 115%
- Reduce time-to-close for enterprise deals from 90 to 60 days
- Grow self-serve signups by 40%

### Level 3: Product Outcomes (Quarterly, Reviewed Biweekly)

Each product team receives or negotiates a product outcome that ladders up to a business outcome. The team has autonomy over how to achieve it.

Example cascade:

| Business Outcome | Product Team | Product Outcome |
|-----------------|-------------|-----------------|
| Increase NRR from 105% to 115% | Engagement team | Increase weekly active usage of reporting dashboards from 30% to 50% of paid accounts |
| Increase NRR from 105% to 115% | Expansion team | Increase percentage of accounts that add a second workspace within 90 days from 12% to 20% |
| Reduce time-to-close from 90 to 60 days | Onboarding team | Reduce median time from signup to first shared report from 14 days to 5 days |

### Level 4: Leading Indicators (Weekly)

Teams break product outcomes into leading indicators they can observe week over week. These are the metrics that tell you whether your experiments and releases are moving the needle before the quarterly product outcome shifts.

Example: If the product outcome is "increase weekly active usage of reporting dashboards from 30% to 50%," leading indicators might be:
- Number of users who create a custom report this week
- Number of users who share a report with a teammate this week
- Percentage of dashboard visitors who return within 48 hours

## Outcome Anti-Patterns

### 1. Too Broad

**Example:** "Improve the user experience."

**Why it fails:** Every possible initiative could qualify. The team cannot prioritize, cannot measure progress, and cannot know when they have succeeded. Broad outcomes give the illusion of alignment while producing scattered efforts.

**Fix:** Narrow to a specific behavior change. "Increase the percentage of new users who complete the 3-step setup wizard from 40% to 65%" is specific enough to drive focused discovery.

### 2. Too Narrow

**Example:** "Increase clicks on the 'Upgrade' button by 20%."

**Why it fails:** This is a solution metric, not an outcome. It constrains the team to a single mechanism (the upgrade button) rather than letting them discover the best path to the underlying goal (more upgrades). It also invites dark patterns.

**Fix:** Step back to the customer behavior you actually want. "Increase the percentage of free users who encounter and recognize the value of a paid feature during their first week" opens space for genuine discovery.

### 3. Vanity Metrics

**Example:** "Reach 1 million registered users."

**Why it fails:** Registration counts include inactive, churned, and fake accounts. The number goes up regardless of product quality. It feels good in a board deck but does not indicate whether customers are getting value.

**Fix:** Replace with an activation or engagement metric. "Reach 100,000 weekly active users who complete at least one core action" is harder to game and reflects real value delivery.

### 4. Lagging-Only Metrics

**Example:** "Reduce annual churn from 15% to 10%."

**Why it fails:** Annual churn is measured once a year (or at best monthly with cohort analysis). By the time the metric moves, 6-12 months of work have passed. Teams cannot learn fast enough to iterate.

**Fix:** Pair lagging metrics with leading indicators. "Reduce the percentage of accounts with zero logins in the past 30 days from 25% to 15%" is a leading indicator of churn that moves weekly and gives the team fast feedback.

### 5. Output Disguised as Outcome

**Example:** "Launch the new onboarding flow by Q2."

**Why it fails:** This is a delivery milestone, not an outcome. It assumes the new onboarding flow will produce the desired result. If it does not, the team has "succeeded" by shipping but failed at creating value.

**Fix:** State the behavior change the onboarding flow is supposed to produce. "Increase the percentage of new users who reach their first value moment within 48 hours from 25% to 45%." Now the team can discover the best way to achieve that, which may or may not involve a full onboarding redesign.

## Examples of Well-Written Product Outcomes

### B2B SaaS (Project Management Tool)

| Business Context | Product Outcome |
|-----------------|-----------------|
| Retention is dropping for mid-market accounts | Increase the percentage of mid-market accounts where 3+ team members are active weekly from 35% to 55% |
| Sales cycle is too long | Reduce median time from free trial start to first project created with real data from 7 days to 2 days |
| Expansion revenue is flat | Increase the percentage of teams that use 3+ integrations within their first 60 days from 18% to 35% |

### Consumer App (Fitness Tracking)

| Business Context | Product Outcome |
|-----------------|-----------------|
| Day-30 retention is 12% | Increase the percentage of new users who log a workout in 3 of their first 7 days from 20% to 40% |
| Subscription conversion is low | Increase the percentage of free users who view their weekly progress summary from 15% to 45% |
| Social features are underused | Increase the percentage of active users who share a workout or milestone with a friend at least once per month from 5% to 20% |

### Internal Tools (Employee HR Portal)

| Business Context | Product Outcome |
|-----------------|-----------------|
| HR team spends 60% of time answering repeat questions | Reduce the percentage of employees who contact HR for information available in the self-service portal from 70% to 30% |
| Benefits enrollment is error-prone | Increase the percentage of employees who complete benefits enrollment without needing to make corrections from 55% to 85% |
| Manager adoption of performance review tool is low | Increase the percentage of managers who complete performance reviews using the tool (vs. offline) from 40% to 80% |

## Template for Writing Product Outcomes

Use this template when defining a product outcome for a team or initiative:

```
PRODUCT OUTCOME TEMPLATE

1. Business outcome this supports:
   [State the company-level metric this ladders up to]

2. Target customer segment:
   [Who specifically are we trying to change behavior for?]

3. Current behavior:
   [What are these customers doing today?]

4. Desired behavior:
   [What do we want them to do instead or in addition?]

5. Product outcome statement:
   Increase/Decrease [specific measurable behavior]
   from [current baseline] to [target]
   for [customer segment]
   by [timeframe].

6. Leading indicators we will track weekly:
   - [Indicator 1]
   - [Indicator 2]
   - [Indicator 3]

7. How we will measure:
   [Data source, instrumentation needed, measurement frequency]

8. Confidence check — answer YES to all:
   [ ] Our product team can directly influence this metric
   [ ] We can measure this at least biweekly
   [ ] This metric changing should plausibly improve the business outcome
   [ ] This is a behavior change, not a feature launch
   [ ] The target is ambitious but not impossible given current trajectory
```

### Filled Example

```
1. Business outcome this supports:
   Increase net revenue retention from 108% to 118%

2. Target customer segment:
   Mid-market accounts (50-500 employees) in their first 90 days

3. Current behavior:
   Only the admin who signed up uses the product actively. Other team
   members have accounts but log in fewer than 2 times per month.

4. Desired behavior:
   At least 3 team members per account are using the product weekly,
   creating and commenting on shared projects.

5. Product outcome statement:
   Increase the percentage of mid-market accounts where 3+ team members
   are active weekly from 35% to 55% by end of Q3.

6. Leading indicators we will track weekly:
   - Number of team invitations sent per new account in first 14 days
   - Percentage of invited users who log in within 48 hours of invitation
   - Number of collaborative actions (comments, shared views) per account per week

7. How we will measure:
   Product analytics (Amplitude), segmented by account size and account age.
   Weekly dashboard review in Friday team sync.

8. Confidence check:
   [x] Our product team can directly influence this metric
   [x] We can measure this at least biweekly
   [x] This metric changing should plausibly improve the business outcome
   [x] This is a behavior change, not a feature launch
   [x] The target is ambitious but not impossible given current trajectory
```

## Negotiating Outcomes with Leadership

Product teams should not passively receive outcomes. The negotiation process matters.

**Step 1: Understand the business context.** Ask leadership: What is the strategic priority? Why now? What does success look like at the business level?

**Step 2: Propose candidate product outcomes.** Come to the conversation with 2-3 product outcomes that you believe ladder up to the business outcome. Include your reasoning and baseline data.

**Step 3: Agree on measurement.** Ensure leadership and the team agree on how the product outcome will be measured, what the current baseline is, and what a reasonable target looks like.

**Step 4: Set review cadence.** Outcomes are not set-and-forget. Agree to review the outcome quarterly. If the team learns through discovery that the product outcome does not actually drive the business outcome, they should be empowered to propose a new one.

**Step 5: Protect team autonomy.** The outcome is the constraint. How the team achieves it — which opportunities to pursue, which solutions to build, which experiments to run — is the team's decision. If leadership dictates solutions, the outcome becomes meaningless.

## When to Change an Outcome

An outcome should change when:

- Discovery reveals the causal link between product outcome and business outcome is weak or nonexistent
- The baseline shifts dramatically (positive or negative) due to external factors
- Company strategy changes and the parent business outcome is replaced
- The team achieves the target and needs a new stretch goal or a new focus area

An outcome should not change when:

- The team is struggling to move the metric (this is a signal to dig deeper into discovery, not to abandon the outcome)
- A stakeholder requests a feature that does not relate to the outcome (redirect the conversation to outcomes)
- The team is bored or wants to work on something else

## Summary

Good outcomes are the foundation of continuous discovery. They constrain the problem space enough to focus the team while leaving enough room for creative solutions. A well-written product outcome is specific, measurable, directly influenceable by the team, observable within weeks, and causally connected to a business outcome. Start with the template, check against the anti-patterns, and negotiate with leadership rather than accepting top-down directives passively.
