# Assumption Testing

Every solution is built on a stack of assumptions. Most of them are invisible until something fails. Assumption testing is the practice of making those assumptions explicit, identifying the riskiest one, and designing fast, cheap experiments to test it before committing to a full build. This guide covers assumption mapping, risk assessment, experiment design across the testing ladder, success criteria, and learning velocity.

## Assumption Mapping: The Four Categories

Every product solution rests on assumptions across four categories. If any category's assumptions are wrong, the solution fails — but it fails for different reasons.

### The Four Categories

| Category | Core Question | If Wrong... |
|----------|--------------|-------------|
| **Desirability** | Do customers want this? | You build something nobody uses. The feature launches to silence. |
| **Viability** | Does this work for our business? | You build something customers love but that loses money, violates regulations, or cannibalizes another product. |
| **Feasibility** | Can we build this? | You commit to a timeline you cannot meet, or discover technical blockers mid-development. |
| **Usability** | Can customers figure out how to use this? | You build something customers want but cannot operate. Adoption stalls despite demand. |

### Generating Assumptions

For each solution, systematically generate assumptions in all four categories. Use these prompts:

**Desirability assumptions:**
- Customers currently experience [specific pain point] frequently enough to want a solution
- Customers would choose this solution over their current workaround
- Customers would choose this solution over [specific competitor alternative]
- This solution addresses the primary need, not a secondary one
- The target segment is large enough to justify investment

**Viability assumptions:**
- We can deliver this at a cost that supports our pricing model
- This does not cannibalize revenue from an existing product or feature
- This aligns with our brand and market position
- We can support this operationally (customer support, infrastructure, legal)
- The revenue or retention impact justifies the development cost

**Feasibility assumptions:**
- The required technology exists and is mature enough for production use
- Our team has (or can acquire) the skills to build this
- We can integrate this with our existing architecture without major refactoring
- We can build this within [timeframe] with [team size]
- Third-party dependencies (APIs, data sources, partners) are reliable and available

**Usability assumptions:**
- Users will understand what this feature does without extensive explanation
- Users can complete the core workflow in [X] steps or fewer
- The feature is discoverable within the existing navigation
- Users with [specific skill level] can use this without training
- Error states are recoverable without support intervention

### Assumption Map Template

```
ASSUMPTION MAP

Solution: [Name/description of the solution]
Opportunity: [The opportunity this solution addresses]
Product Outcome: [The product outcome this supports]

DESIRABILITY
D1: [Assumption]
D2: [Assumption]
D3: [Assumption]

VIABILITY
V1: [Assumption]
V2: [Assumption]
V3: [Assumption]

FEASIBILITY
F1: [Assumption]
F2: [Assumption]
F3: [Assumption]

USABILITY
U1: [Assumption]
U2: [Assumption]
U3: [Assumption]
```

## Identifying the Riskiest Assumption

Not all assumptions are equally dangerous. The riskiest assumption is the one that is most likely to be wrong AND would cause the most damage if wrong.

### The Risk Assessment Matrix

Plot each assumption on two dimensions:

| | Low Impact if Wrong | High Impact if Wrong |
|---|---|---|
| **Likely True** | Low risk — skip or test later | Medium risk — test if cheap |
| **Uncertain or Likely False** | Medium risk — monitor | **HIGH RISK — test first** |

### How to Assess Likelihood

Ask yourself these questions for each assumption:

- **Do we have any evidence for or against this?** Direct evidence (customer interviews, data, past experiments) beats intuition.
- **Is this a known pattern or a novel bet?** If your assumption relies on customers behaving in a way they have never behaved before, it is likely uncertain.
- **Do team members disagree about this?** Disagreement is a signal of uncertainty. If the PM thinks customers want this but the designer is skeptical, that assumption needs testing.
- **Have we or competitors tried something similar?** Past failures in adjacent spaces are evidence against. Past successes are evidence for.

### How to Assess Impact

- **Is this a load-bearing assumption?** If this assumption is wrong, does the entire solution collapse, or can we adapt?
- **Is the cost of being wrong recoverable?** Building a feature for 3 months based on a wrong desirability assumption is costly. Running a 1-week experiment based on the same wrong assumption is cheap.
- **Does this assumption affect other solutions too?** If assumption D1 is wrong, and it also undermines Solutions B and C, the impact cascades.

### Worked Example

Solution: Invite-gated collaborative dashboard feature for trial users.

| ID | Assumption | Category | Likely True? | Impact if Wrong | Risk Level |
|----|-----------|----------|:---:|:---:|:---:|
| D1 | Trial users want to collaborate with teammates during the trial | Desirability | Uncertain | High — entire solution premise | **HIGH** |
| D2 | A shared dashboard is the most compelling collaborative feature | Desirability | Uncertain | Medium — could swap feature | Medium |
| V1 | Gating a feature behind invites will not increase trial churn | Viability | Uncertain | High — could hurt conversion | **HIGH** |
| F1 | We can implement feature gating within 1 sprint | Feasibility | Likely true | Low — small scope | Low |
| U1 | Users will understand what the locked feature does from the preview | Usability | Uncertain | Medium — could add explanation | Medium |

Riskiest assumptions to test first: D1 and V1. Test D1 before building anything. Test V1 with a small cohort before full rollout.

## The Testing Ladder

Experiments range from fast-and-cheap to slow-and-definitive. The testing ladder organizes them by fidelity and cost. Always start at the lowest rung that can adequately test your riskiest assumption.

### Rung 1: One-Question Survey or Poll

**What it is:** A single targeted question delivered to existing users via in-app prompt, email, or existing touchpoint.

**Best for testing:** Desirability assumptions at a surface level. Gauging interest, frequency of a problem, or awareness of a need.

**Time to run:** 1-3 days

**Template:**

```
SURVEY EXPERIMENT

Assumption being tested: [e.g., D1: Trial users want to collaborate
  with teammates during the trial]
Question: "During your trial, how important is it to you to work with
  teammates inside [Product]?"
Answer options: Not at all important / Slightly important / Moderately
  important / Very important / Essential
Audience: 200 trial users who signed up in the last 14 days
Success criterion: 40%+ select "Very important" or "Essential"
Timeline: Send Monday, analyze Wednesday
```

**Limitations:** Self-reported interest does not equal behavior. Use as a directional signal, not proof.

### Rung 2: Fake Door / Painted Door Test

**What it is:** Add a button, menu item, or UI element for a feature that does not exist yet. Measure how many people click it. Show a message explaining the feature is coming soon and optionally collect email signups.

**Best for testing:** Desirability assumptions. Measures actual behavioral intent, not stated preference.

**Time to run:** 3-7 days

**Template:**

```
FAKE DOOR EXPERIMENT

Assumption being tested: [e.g., D2: A shared dashboard is the most
  compelling collaborative feature]
Implementation: Add "Share Dashboard" button to the dashboard view.
  On click, show modal: "Shared Dashboards are coming soon! Enter your
  email to be first to try it."
Audience: All active trial users for 7 days
Primary metric: Click-through rate on the button
Secondary metric: Email signup rate on the modal
Success criterion: 8%+ CTR (based on baseline feature engagement rates)
Timeline: Deploy Monday, measure for 7 days, analyze next Monday
```

**Limitations:** Clicking a button is not the same as sustained usage. A fake door tests initial interest, not ongoing value.

### Rung 3: Prototype Test

**What it is:** A non-functional or minimally functional version of the solution (Figma prototype, clickable wireframe, or a stripped-down working version) tested with 5-8 real users in moderated sessions.

**Best for testing:** Usability assumptions and deeper desirability assumptions. Do users understand the concept? Can they complete the workflow? Does it feel valuable?

**Time to run:** 1-2 weeks (design + recruit + test + analyze)

**Template:**

```
PROTOTYPE EXPERIMENT

Assumption being tested: [e.g., U1: Users will understand what the
  locked feature does from the preview]
Prototype: Figma clickable prototype showing the locked dashboard
  preview and the invite-to-unlock flow
Participants: 6 trial users recruited from recent signups
Tasks:
  1. "You've just logged in. Explore the dashboard area and tell me
     what you see."
  2. "What do you think 'Share Dashboard' does?"
  3. "Walk me through how you would get access to this feature."
Observation criteria:
  - Can participants identify what the locked feature does? (Y/N)
  - Do participants understand the invite-to-unlock mechanism? (Y/N)
  - What is their emotional reaction? (positive / neutral / negative)
Success criterion: 5 of 6 participants correctly identify the feature
  purpose and understand the unlock mechanism
Timeline: Design prototype (3 days), recruit (2 days), test (3 days),
  analyze (1 day)
```

### Rung 4: Concierge Test

**What it is:** Deliver the value proposition manually, without building the actual product feature. A human performs the work that the product would eventually automate.

**Best for testing:** Desirability and viability assumptions simultaneously. Do customers actually use the service when it exists? Is the value real enough to justify the investment?

**Time to run:** 1-4 weeks

**Template:**

```
CONCIERGE EXPERIMENT

Assumption being tested: [e.g., D1: Trial users want to collaborate
  with teammates during the trial]
Implementation: For the next 20 trial signups, a CS rep personally
  reaches out on day 2 and offers to help them set up a shared
  workspace with their team. The CS rep manually creates the shared
  view and sends invitations on behalf of the user.
Audience: 20 consecutive trial signups meeting ICP criteria
Primary metric: Percentage of users who accept the offer
Secondary metric: Percentage of invited teammates who join
Tertiary metric: Trial-to-paid conversion rate for this cohort vs. control
Success criteria:
  - 50%+ accept the collaboration setup offer
  - 30%+ of invited teammates join
  - Conversion rate is at least 1.5x the control group
Timeline: 2 weeks of enrollment, 2 weeks of observation
```

**Limitations:** Does not test feasibility or scalability. The solution may work manually but be impossible to automate economically.

### Rung 5: A/B Test (Live Experiment)

**What it is:** Build a minimal working version of the feature and deploy it to a randomized subset of users. Compare behavior against a control group.

**Best for testing:** All four assumption categories simultaneously, with statistical rigor.

**Time to run:** 2-6 weeks (build + run + reach statistical significance)

**Template:**

```
A/B TEST EXPERIMENT

Assumption being tested: [e.g., V1: Gating a feature behind invites
  will not increase trial churn]
Variants:
  - Control (50%): Standard trial experience, no feature gating
  - Treatment (50%): Shared dashboard visible but locked behind
    teammate invitation
Audience: All new trial signups for 4 weeks (estimated 400 per variant)
Primary metric: Trial-to-paid conversion rate
Secondary metrics:
  - Teammate invitation rate
  - Trial churn rate (account deletion or zero logins after day 7)
  - Feature engagement rate (for treatment group)
Minimum detectable effect: 3 percentage points on conversion rate
Required sample size: 800 total (400 per variant)
Success criteria:
  - Treatment conversion rate is not lower than control (non-inferiority)
  - Treatment invitation rate is at least 2x control
  - Trial churn rate does not increase by more than 2 percentage points
Timeline: 4 weeks of enrollment + 2 weeks of observation post-trial end
```

### Choosing the Right Rung

| Riskiest Assumption Type | Start At |
|--------------------------|----------|
| "Do customers even have this problem?" | Rung 1 (survey) or customer interviews |
| "Would customers engage with this?" | Rung 2 (fake door) |
| "Can customers use this?" | Rung 3 (prototype) |
| "Will customers get real value from this?" | Rung 4 (concierge) |
| "Does this work at scale without negative side effects?" | Rung 5 (A/B test) |

Move up the ladder only when the current rung gives you a positive signal. A negative signal at any rung means you should reconsider the assumption, the solution, or the opportunity — not jump to a higher-fidelity test hoping for a different answer.

## Setting Success Criteria Before Testing

This is the most violated principle in experimentation. Teams run experiments, look at the results, and then decide whether they are good enough. This is backwards and invites confirmation bias.

### Pre-Registration Protocol

Before running any experiment, document:

1. **The assumption being tested** (stated as a falsifiable claim)
2. **The metric(s) you will measure**
3. **The threshold for success** (a specific number, not "significant improvement")
4. **The threshold for failure** (a specific number below which you will abandon or rethink)
5. **The decision you will make based on each outcome:**
   - If success: [next step]
   - If failure: [next step]
   - If inconclusive: [next step]

### Example Pre-Registration

```
PRE-REGISTRATION

Assumption: Trial users want to collaborate with teammates during
  the trial (D1)
Experiment: Fake door test — "Share Dashboard" button
Metric: Click-through rate (CTR) on the button over 7 days
Success threshold: CTR >= 8%
Failure threshold: CTR < 3%
Inconclusive range: 3-8% CTR

Decision tree:
  - If CTR >= 8%: Proceed to prototype test for usability (Rung 3)
  - If CTR < 3%: Abandon this solution. Return to opportunity tree
    and re-evaluate whether collaboration during trial is the right
    opportunity to pursue.
  - If CTR 3-8%: Inconclusive. Run for 7 more days with a larger
    sample. If still in this range, interview 5 users who clicked
    to understand their motivation before deciding.
```

### How to Set Thresholds

- **Use baselines.** If your average feature engagement CTR is 5%, an 8% threshold means this feature is more compelling than average. A 3% threshold means it is below average.
- **Use comparable experiments.** If previous fake door tests for features you shipped averaged 10% CTR, set your threshold relative to that.
- **Use business math.** If you need 25% of trial users to invite teammates to hit your product outcome, and your invite flow conversion rate is 50%, you need 50% of users to reach the invite flow — so your fake door CTR needs to be at least 50%. Work backwards from the outcome.
- **When in doubt, be conservative.** It is better to kill a mediocre idea early than to invest months discovering it was mediocre all along.

## Learning Velocity Metrics

The goal of continuous discovery is not just to run experiments — it is to learn faster than the competition. Track these metrics to ensure your testing practice is healthy.

### Metrics to Track

| Metric | What It Measures | Target |
|--------|-----------------|--------|
| **Experiments per week** | Throughput of your testing practice | 1+ per product trio per week |
| **Time from assumption to first test result** | Speed of the feedback loop | Less than 2 weeks for Rungs 1-3 |
| **Percentage of tests with pre-registered success criteria** | Discipline of experimental practice | 100% |
| **Kill rate** | Percentage of ideas abandoned based on test results | 30-60% (lower means you are not testing risky enough assumptions; higher means you are not generating good enough ideas) |
| **Assumption coverage** | Percentage of high-risk assumptions that have been tested before code is committed | 80%+ |
| **Pivot rate** | How often test results change the team's direction | Track qualitatively — zero pivots means you are only testing safe assumptions |

### Interpreting Learning Velocity

**Low experiments per week (< 1):** The team is probably spending too long designing experiments, waiting for perfect sample sizes, or running experiments sequentially instead of in parallel. Fix by defaulting to lower rungs of the testing ladder and accepting directional signals.

**High kill rate (> 60%):** The team is generating solutions without sufficient connection to validated opportunities. Return to opportunity discovery and ensure solutions are grounded in interview data.

**Low kill rate (< 30%):** The team is testing assumptions they already believe are true. This is confirmation theater, not discovery. Challenge the team to test the assumption they are least sure about.

**Long time to first result (> 2 weeks for simple tests):** Operational friction is slowing down learning. Common culprits: slow recruitment, over-designed experiments, waiting for statistical significance on directional tests, or requiring too many approvals.

## Assumption Testing in Practice: A Weekly Rhythm

| Day | Activity |
|-----|----------|
| **Monday** | Review last week's experiment results. Update assumption map. Decide next riskiest assumption. |
| **Tuesday** | Design the experiment. Write pre-registration. Prepare materials (survey, fake door, prototype). |
| **Wednesday** | Launch the experiment. |
| **Thursday-Friday** | Monitor early signals (for multi-day experiments). Run interviews or prototype tests (for same-week experiments). |
| **Following Monday** | Analyze results. Make the pre-registered decision. Start the cycle again. |

This rhythm means the team is always running at least one experiment. Over a quarter (12-13 weeks), a team running one experiment per week generates 12-13 data points about their assumptions. Compare that to a team that builds features for 6 weeks and then measures impact — they get 2 data points in the same period.

## Summary

Assumption testing transforms product development from a series of bets into a series of informed decisions. Map assumptions across all four categories (desirability, viability, feasibility, usability). Identify the riskiest one using impact-and-likelihood analysis. Design the smallest, cheapest experiment that can test it using the appropriate rung of the testing ladder. Set success criteria before looking at results. Track learning velocity to ensure your practice is fast and honest. The team that tests assumptions weekly will outlearn and outperform the team that ships features quarterly and hopes for the best.
