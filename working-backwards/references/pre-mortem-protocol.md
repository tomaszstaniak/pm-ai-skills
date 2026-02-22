# Pre-Mortem Protocol

A post-mortem asks "what went wrong?" after a project fails. A pre-mortem asks "what went wrong?" before the project launches — by imagining that it has already failed and working backward to identify the causes. This inversion turns a speculative question ("what could go wrong?") into a retrospective question ("what did go wrong?"), and the difference in framing has a measurable impact on the quality of thinking.

## The Research Behind Pre-Mortems

Gary Klein, a research psychologist specializing in decision-making, developed the pre-mortem technique based on research into prospective hindsight. The foundational study by Mitchell, Russo, and Pennington (1989) found that imagining an event has already occurred increases the ability to identify reasons for that event by approximately 30% compared to imagining it might occur in the future.

The mechanism is straightforward. When you ask "what could go wrong?" people engage in cautious speculation. They hedge. They stay general. They unconsciously filter for plausibility and social acceptability. When you say "the project has failed — tell me why," people engage a different cognitive mode. They generate specific, concrete causes. They feel permission to name uncomfortable truths because they are explaining a fact, not making a prediction.

Klein also identified a critical social dynamic: in conventional risk assessment, team members with concerns often self-censor because raising problems can be perceived as being negative or unsupportive. The pre-mortem reframes problem identification as a competitive analytical exercise. The person who identifies the most likely failure cause is seen as insightful, not obstructive.

### Why Pre-Mortems Work Better Than Risk Brainstorming

| Traditional Risk Assessment | Pre-Mortem |
|---|---|
| "What could go wrong?" | "The project failed. Why?" |
| Speculative, future-oriented framing | Retrospective, past-oriented framing |
| Participants hedge and stay general | Participants generate specific, concrete causes |
| Social pressure to be positive | Social permission to be critical |
| Produces a list of generic risks | Produces a list of specific, scenario-based failures |
| Often dominated by the loudest voices | Individual generation before group discussion |
| Feels like an obligation | Feels like a puzzle |

## Step-by-Step Facilitation Guide

### Before the Session

**Who should participate:** The core product team plus two to three people outside the team who have relevant expertise or a fresh perspective. Include at least one person who has been through a similar project that failed. Ideal group size is six to ten people.

**What to distribute in advance:** The PR/FAQ document. Participants should have read it thoroughly before the session. The pre-mortem is not the place to learn about the project for the first time.

**Time required:** 90 minutes. Do not compress this into 60 minutes. The individual generation phase needs space.

**Materials:** Sticky notes or index cards (physical or digital), a timer, a whiteboard or shared document for clustering.

### Session Structure

#### Phase 1: Setup (5 minutes)

The facilitator reads the following statement aloud:

> "Imagine that it is [12 months / 18 months / appropriate timeframe] from now. We launched the product described in the PR/FAQ. It failed. Not a partial setback — a clear failure. The product has been shut down, or usage is a fraction of what we projected, or the team has been reassigned to other projects. Your job is to explain why it failed. Work individually and generate as many specific failure causes as you can. Be concrete. Do not write 'the market changed' — write a specific scenario of how and why the market shifted in a way that killed this product."

Emphasize: there is no wrong answer. The more causes generated, the better. Quantity over quality in this phase.

#### Phase 2: Individual Generation (10 minutes)

Each participant works alone to generate failure causes. One cause per card or sticky note. Enforce silence during this phase — no discussion, no collaboration. This prevents anchoring and groupthink.

**Coaching tips for participants:**
- Think about failures you have seen in past projects and whether similar dynamics apply here
- Consider each stakeholder group: customers, partners, internal teams, competitors, regulators
- Think about the assumptions in the PR/FAQ — what if each one is wrong?
- Consider both dramatic failures (competitor launches a free alternative) and slow failures (adoption curve is 60% of projection)

#### Phase 3: Round-Robin Sharing (20 minutes)

Go around the room. Each person shares one failure cause. Continue cycling through the group until all causes have been shared. The facilitator captures each cause on a shared board.

**Rules for this phase:**
- No discussion or debate during sharing
- No "that is the same as mine" — if two causes sound similar, share both. Nuances matter.
- The facilitator may ask clarifying questions but not evaluative ones
- Duplicates will be merged later

#### Phase 4: Clustering and Discussion (25 minutes)

Group the failure causes into categories (see the taxonomy below). Discuss each cluster:
- Which causes in this cluster are most likely?
- Which would be most damaging?
- Are any of these causes already showing warning signs?

This is the phase where debate is encouraged. The goal is not consensus — it is shared understanding of the risk landscape.

#### Phase 5: Scoring (15 minutes)

For each failure cause (or cluster), assign two scores:

**Likelihood:** How probable is this failure mode?

| Score | Label | Meaning |
|---|---|---|
| 1 | Very unlikely | Would require multiple improbable events |
| 2 | Unlikely | Possible but would need specific conditions |
| 3 | Possible | Could happen under normal circumstances |
| 4 | Likely | Expected unless we actively prevent it |
| 5 | Very likely | Will almost certainly happen without intervention |

**Impact:** If this failure mode occurs, how severe is the damage?

| Score | Label | Meaning |
|---|---|---|
| 1 | Minimal | Minor setback, easily recovered |
| 2 | Low | Noticeable delay or cost increase |
| 3 | Moderate | Significant impact on timeline, budget, or outcomes |
| 4 | High | Project success is seriously threatened |
| 5 | Critical | Project failure is near-certain if this occurs |

**Scoring matrix:**

|  | Impact 1 | Impact 2 | Impact 3 | Impact 4 | Impact 5 |
|---|---|---|---|---|---|
| **Likelihood 5** | 5 | 10 | 15 | 20 | 25 |
| **Likelihood 4** | 4 | 8 | 12 | 16 | 20 |
| **Likelihood 3** | 3 | 6 | 9 | 12 | 15 |
| **Likelihood 2** | 2 | 4 | 6 | 8 | 10 |
| **Likelihood 1** | 1 | 2 | 3 | 4 | 5 |

**Risk tiers:**
- **Score 15-25 (Critical):** Must have a mitigation plan before proceeding. If mitigation is not credible, this is a potential project-stopper.
- **Score 8-14 (Significant):** Requires a mitigation plan and ongoing monitoring.
- **Score 4-7 (Moderate):** Should have a contingency plan documented.
- **Score 1-3 (Low):** Acknowledge and monitor. No active mitigation required.

#### Phase 6: Mitigation Planning (15 minutes)

For every risk in the Critical and Significant tiers, define:

1. **Prevention actions:** What can we do now to reduce the likelihood?
2. **Detection signals:** What early indicators would tell us this risk is materializing?
3. **Response plan:** If this risk materializes despite prevention, what is our response?
4. **Owner:** Who is responsible for monitoring and responding?

Use the mitigation planning template below.

## Failure Category Taxonomy

When clustering failure causes, use these categories. Most pre-mortems surface failures in four to six of these categories. If a category has zero failure causes, either the project has no risk in that area (unlikely) or the team has a blind spot (far more likely).

### 1. Customer Failures

The product works as designed but customers do not want it, do not use it, or do not value it enough to pay.

**Common patterns:**
- The problem is real but not painful enough to motivate behavior change
- The target customer segment is too small or too hard to reach
- Customers say they want it in research but do not adopt it in practice
- The product solves the problem but creates new problems that offset the benefit
- Price sensitivity is higher than expected

### 2. Market Failures

External market conditions undermine the product's viability.

**Common patterns:**
- A well-funded competitor launches a similar or better solution
- A platform shift (regulatory, technological, economic) changes the landscape
- The market window closes before the product is ready
- A free or open-source alternative emerges
- An adjacent incumbent adds the capability as a feature of their existing product

### 3. Execution Failures

The team cannot build what was promised, on time or at the required quality level.

**Common patterns:**
- Technical complexity was underestimated
- Key dependencies (APIs, partnerships, infrastructure) were not secured
- The team lacked critical skills and hiring took longer than planned
- Scope crept beyond what the timeline and budget could support
- Quality issues required extensive rework

### 4. Business Model Failures

The product works and customers use it, but the economics do not support a viable business.

**Common patterns:**
- Customer acquisition cost is higher than expected
- Willingness to pay is lower than assumed
- Churn rate makes LTV insufficient to justify CAC
- Infrastructure costs scale faster than revenue
- The product requires ongoing human intervention that does not scale

### 5. Adoption Failures

The product is good but adoption stalls due to friction, switching costs, or behavioral inertia.

**Common patterns:**
- Onboarding is too complex for the target user
- The product requires changing established workflows or habits
- Network effects are needed but the cold-start problem is not solved
- The product requires organizational buy-in that individual users cannot secure
- Integration with existing tools is insufficient

### 6. Internal Failures

Organizational dynamics prevent the project from succeeding regardless of market or product quality.

**Common patterns:**
- Leadership support is withdrawn due to changing priorities
- Key team members leave and replacements are not available
- Internal politics block access to required resources or partnerships
- The project conflicts with another team's priorities
- Decision-making is too slow and the project misses critical windows

## Mitigation Planning Template

For each Critical or Significant risk:

```
RISK: [Specific failure cause]
CATEGORY: [Customer / Market / Execution / Business Model / Adoption / Internal]
LIKELIHOOD: [1-5]  IMPACT: [1-5]  SCORE: [L x I]

PREVENTION ACTIONS:
1. [Action] — Owner: [Name] — By: [Date]
2. [Action] — Owner: [Name] — By: [Date]

DETECTION SIGNALS:
- [Leading indicator that this risk is materializing]
- [Second indicator]
- Monitoring frequency: [Daily / Weekly / Monthly]

RESPONSE PLAN:
If detected, we will:
1. [Immediate action]
2. [Escalation path]
3. [Decision point: continue / pivot / stop]

TRIPWIRE:
If [specific metric] reaches [threshold] by [date], we will [specific action].

OWNER: [Name responsible for monitoring this risk]
```

**Example completed template:**

```
RISK: Primary API partner increases pricing by 3x or more, making unit economics unviable.
CATEGORY: Business Model / Market
LIKELIHOOD: 3  IMPACT: 4  SCORE: 12

PREVENTION ACTIONS:
1. Negotiate 18-month pricing commitment before launch — Owner: Sarah — By: March 15
2. Build abstraction layer to enable provider switching — Owner: James — By: April 30
3. Identify and test two backup providers — Owner: James — By: May 15

DETECTION SIGNALS:
- API partner announces pricing changes to any customer tier
- API partner is acquired or raises funding at valuation implying monetization pressure
- Monitoring frequency: Monthly check on partner's public announcements and pricing page

RESPONSE PLAN:
If detected, we will:
1. Immediately begin integration testing with backup provider (1-week sprint)
2. Model revised unit economics with backup provider pricing
3. If no viable alternative exists, present revised economics to leadership within 2 weeks

TRIPWIRE:
If API costs exceed 25% of revenue at any point, we will initiate provider migration within 30 days.

OWNER: Sarah (business), James (technical)
```

## Using Pre-Mortem Results in Go/No-Go Decisions

The pre-mortem does not make the decision. It informs the decision. After completing the pre-mortem, present the results to leadership alongside the PR/FAQ using this framework:

### Decision Input Summary

**Total risks identified:** [Number]

**Risk distribution:**

| Tier | Count | Mitigatable | Unmitigatable |
|---|---|---|---|
| Critical (15-25) | | | |
| Significant (8-14) | | | |
| Moderate (4-7) | | | |
| Low (1-3) | | | |

**Key findings:**
1. [Biggest risk and proposed mitigation]
2. [Second biggest risk and proposed mitigation]
3. [Any risk that is unmitigatable and must be accepted]

**Recommendation:** One of the following:
- **Proceed:** Risks are understood, mitigations are credible, the opportunity justifies the risk.
- **Proceed with conditions:** Specific milestones or tripwires must be met before full commitment.
- **Revisit:** One or more critical risks do not have credible mitigations. The team needs more time to resolve specific questions.
- **Do not proceed:** Unmitigatable risks are too high relative to the opportunity.

### When to Re-Run the Pre-Mortem

A pre-mortem is not a one-time exercise. Re-run it when:

- The scope of the project changes significantly
- A major assumption is invalidated (e.g., a key partnership falls through)
- The competitive landscape shifts materially
- The team composition changes substantially
- The project passes a major milestone and is about to enter the next phase

Each subsequent pre-mortem should review the original risk register: which risks materialized, which mitigations worked, and what new risks have emerged. This creates an evolving risk document that improves decision quality throughout the project lifecycle.

## Common Facilitation Mistakes

| Mistake | Why It Fails | Fix |
|---|---|---|
| Skipping the individual generation phase | Group brainstorming produces fewer and less diverse ideas due to anchoring and social pressure | Enforce 10 minutes of silent individual work before any sharing |
| Allowing debate during the sharing phase | People stop generating new ideas when they are defending existing ones | Strictly separate generation from evaluation |
| Letting the project champion facilitate | The champion has an incentive to minimize risks, even unconsciously | Use a neutral facilitator who has no stake in the project's approval |
| Stopping at risk identification without scoring | An unscored list of 40 risks is overwhelming and not actionable | Always score and tier the risks |
| Treating the pre-mortem as a checklist exercise | Going through the motions without genuine engagement produces generic risks | Emphasize that the pre-mortem exists to protect the team, not to block the project |
| Not documenting mitigation owners and dates | Mitigations without owners do not get executed | Every Critical and Significant risk must have a named owner and a deadline |
