# Prioritization Methods

Prioritization is where most discovery work goes to die. Teams generate dozens of opportunities and ideas, then collapse back to "what feels important" or "what the loudest stakeholder wants." This guide covers structured methods for choosing what to pursue next — methods that surface real tradeoffs, force explicit comparisons, and avoid the analysis paralysis that turns discovery into a stalling tactic.

## The Core Principle: Compare, Don't Score

The single most important shift in opportunity prioritization is to **compare opportunities head-to-head rather than score them in isolation**. When you score opportunities independently, almost everything ends up looking like a 4 out of 5. When you force a direct comparison — "if we could only do one of these, which would it be?" — the team must articulate the actual reasoning behind their preference, and the disagreements that surface are the most valuable signal in the room.

Independent scoring produces consensus. Head-to-head comparison produces clarity.

## When to Prioritize

Prioritization happens at three layers of the Opportunity Solution Tree, and the right method differs at each:

| Layer | What you are choosing between | Recommended method |
|-------|-------------------------------|--------------------|
| **Opportunities** | Which customer need to address next | Head-to-head comparison + frequency / severity / outcome alignment |
| **Solutions** | Which approach to take for a chosen opportunity | Compare-and-contrast on effort / impact / assumption risk |
| **Assumption tests** | Which test to run first | Riskiest-assumption-first; cheapest-falsifying-test |

This guide focuses on the opportunity layer. See `solution-generation.md` and `assumption-testing.md` for the other layers.

## Method 1: Frequency × Severity × Outcome Alignment

The default scoring framework introduced in `opportunity-discovery.md` works as a starting point for triage. Score each opportunity on three dimensions:

| Dimension | Question | Scale |
|-----------|----------|-------|
| **Frequency** | How often do customers encounter this problem? | 1 (rarely) → 5 (daily or more) |
| **Severity** | How painful is it when they encounter it? | 1 (minor annoyance) → 5 (blocking failure) |
| **Outcome alignment** | How directly does solving this move our product outcome? | 1 (loosely connected) → 5 (directly drives the metric) |

Multiply for a priority score (max 125). The score is a **heuristic to drive conversation**, not a number to optimize. If the team agrees on the scores, the conversation is more valuable than the math.

### Worked Example

Product outcome: increase 30-day retention from 28% to 38% for a B2C meditation app.

| Opportunity | Freq | Sev | Align | Score |
|-------------|------|-----|-------|-------|
| Users forget to meditate on busy days | 5 | 3 | 5 | 75 |
| Algorithm shows popular sessions, not personalized ones | 3 | 3 | 3 | 27 |
| Users feel no sense of progress | 4 | 4 | 5 | 80 |
| Want to meditate with partner | 2 | 3 | 2 | 12 |
| Free-tier paywall too aggressive | 4 | 4 | 4 | 64 |

Initial ranking: progress (80) → forget (75) → paywall (64) → algorithm (27) → partner (12).

But this is only the starting point. Use it to anchor the head-to-head conversation.

## Method 2: Head-to-Head Bracket

Once you have a triage ranking, force pairwise comparisons. The bracket method works best:

1. Take the top 5-7 opportunities from triage scoring.
2. Pair them. For each pair, the trio must answer: *"If we could only address one of these, which would it be, and why?"*
3. Eliminate the loser of each pair.
4. Repeat with survivors until one opportunity remains.

The reasoning that surfaces during the pairwise rounds is the real output, not the winner. Capture the rationale for each elimination — it becomes the documentation for why you are not pursuing the other opportunities.

### Worked Example: Bracket Round

Pair 1: "Users feel no sense of progress" (80) vs. "Users forget on busy days" (75)
- Argument for progress: addresses an emotional driver that, once solved, increases the *value* of meditating, not just the *frequency*. Likely to compound.
- Argument for forget: easier to test, faster to ship, larger affected user base.
- **Trio decision:** Progress. The team believes solving forgetting without solving the underlying motivation (progress) produces short-term DAU lift but does not change long-term retention. Notification engineering would be wasted if the underlying perceived value is low.

Pair 2: "Paywall too aggressive" (64) vs. "Algorithm not personalized" (27)
- **Trio decision:** Paywall. Higher signal density, larger affected population, clearer outcome connection.

Final: "No sense of progress" vs. "Paywall too aggressive"
- **Trio decision:** No sense of progress. Paywall is a pricing/PM issue solvable without engineering investment in the next cycle. Progress is the harder, more strategic bet.

The bracket forces the team to articulate a *theory of value* — "engagement compounds when users perceive growth" — rather than just ranking pain levels.

## Method 3: ICE for Quick Triage

When you have many opportunities and need to thin the field fast, ICE is faster than the F×S×A framework:

| Dimension | Question | Scale |
|-----------|----------|-------|
| **Impact** | If we solve this perfectly, how much does it move our outcome? | 1-10 |
| **Confidence** | How sure are we that this is real and solvable? | 1-10 |
| **Ease** | How simple would it be to test the riskiest assumption? | 1-10 |

Average the three for a single score. Use ICE only for triage; switch to F×S×A or head-to-head when narrowing the top 3-5.

## Method 4: RICE for Cross-Team Comparison

When prioritizing opportunities that affect different parts of the product or different teams, RICE introduces a population-weighting factor:

| Dimension | Definition |
|-----------|-----------|
| **Reach** | Number of users affected per quarter |
| **Impact** | Effect on the user's outcome per user (rough estimate: 0.25 / 0.5 / 1 / 2 / 3) |
| **Confidence** | Percentage confidence in your impact and reach estimates |
| **Effort** | Person-months required to test or solve |

`RICE = (Reach × Impact × Confidence) / Effort`

RICE is useful when comparing across product surfaces ("Should we work on onboarding or the dashboard?"). It is overkill for within-surface comparison and tends to bias toward features that touch many users over features that deeply change behavior for a smaller group — which can be the wrong bet for a retention or activation outcome.

## Beyond Scoring: Considerations the Framework Misses

Numerical methods miss factors that experienced product trios know matter. Always sanity-check the score with these questions:

### Strategic Alignment

Does this opportunity align with where the company is going, not just where it is today? An opportunity scoring 60 today that aligns with the company's stated direction in 18 months may be more valuable than an opportunity scoring 80 in a part of the product the company plans to deprecate.

### Existing Evidence

Opportunities with more interview convergence are less risky to pursue. An opportunity mentioned by 9 of 12 interviewees is more validated than one mentioned by 2 of 12 — even if the latter scores higher on severity.

### Segment Concentration

Where does this opportunity cluster? An opportunity that affects only a strategically critical segment (e.g., enterprise customers worth 80% of revenue) may deserve elevation even if it scores lower in aggregate.

### Solution Space Maturity

How many distinct solution directions exist for this opportunity? If you have only one obvious solution candidate, the opportunity is risky — you will likely build the obvious thing without comparison. Opportunities with multiple plausible solutions enable real compare-and-contrast.

### Dependencies

Some opportunities cannot be solved until others are addressed first. Map dependencies before committing to a sequence. A sequence that solves a prerequisite opportunity even if it scores lower may unlock the higher-scoring opportunity downstream.

### Existing Momentum

If the team is already adjacent to a problem space — with data, customer context, partial solutions — the cost-to-test is lower than the raw effort estimate suggests. This is a legitimate reason to pursue an opportunity that scores slightly lower.

## Common Prioritization Mistakes

### Mistake 1: Letting the Loudest Stakeholder Set the Agenda

The most common form of prioritization is unconscious deference to whichever stakeholder pushed hardest in the last meeting. This produces a portfolio that looks like a feature list of stakeholder requests, not a strategy.

**Fix:** Always anchor prioritization in the desired outcome. Force the question: "Which opportunity, if solved, will move the metric the most?" Stakeholder pressure that cannot answer that question goes into the backlog, not the active set.

### Mistake 2: Recency Bias

Whatever the last customer said tends to feel like the most important thing. Three calls later, a different opportunity feels most important.

**Fix:** Score and compare opportunities only with the full opportunity tree visible. Insist on at least 6-8 interview data points per opportunity before treating it as validated.

### Mistake 3: Optimization Paralysis

Some teams treat prioritization as a problem to solve perfectly. They build elaborate spreadsheets, weight every factor, run sensitivity analyses, and never decide. Three weeks pass with no learning.

**Fix:** The goal of prioritization is to make a *good-enough* decision quickly so the team can learn. A method that takes 60 minutes to converge produces faster learning than a method that takes 6 hours. Optimize for cycle time, not perfect ranking.

### Mistake 4: Mistaking Effort Estimates for Truth

"Effort" in any prioritization framework is a guess, especially early in discovery when solutions have not been designed. Teams routinely under-estimate work by 2-5x.

**Fix:** Treat effort estimates as a tie-breaker, not a primary input. Prioritize on opportunity value first. Use effort to choose between two roughly equivalent opportunities, not to demote a high-value opportunity that looks expensive.

### Mistake 5: Never Revisiting Prioritization

Teams rank opportunities at the start of a quarter and treat the ranking as fixed for 12 weeks. By week 4, new interview data has invalidated the rationale, but the ranking persists out of inertia.

**Fix:** Revisit prioritization every 2-4 weeks as new evidence accumulates. Make it a calendar event. Most rankings will be confirmed; some will shift, and the shifts are where learning is happening.

### Mistake 6: Confusing Prioritization with Sequencing

These are different decisions. Prioritization picks the most important opportunity. Sequencing picks the *order* in which to work on the top 3-5. Sometimes the highest-priority opportunity should not be worked on first because a lower-priority opportunity unlocks it or has a faster learning cycle.

**Fix:** First decide priority. Then decide sequence as a separate conversation with explicit reasoning. Document both.

## Connecting Prioritization to the Weekly Discovery Cadence

Prioritization is not a quarterly event. It is a weekly conversation that produces small adjustments. The trio's Friday review should include:

1. **What did we learn this week?** New evidence from interviews, experiment results, or product analytics.
2. **Does anything in our top 5 need to move?** Up, down, or off the list.
3. **What is the highest-leverage thing we can do next week given current rankings?**

Most weeks the answer is "no change." But the act of asking surfaces shifts before they become significant, and keeps the OST aligned with reality.

## Summary

Good prioritization compares opportunities head-to-head rather than scoring them in isolation. Use F×S×A or ICE for initial triage, then run head-to-head brackets on the top 5-7. Sanity-check scores against strategic alignment, evidence depth, segment concentration, solution maturity, and dependencies. Make decisions quickly to maximize learning cycles, and revisit rankings continuously as new evidence accumulates.
