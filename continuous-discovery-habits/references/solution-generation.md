# Solution Generation

Once you have identified and prioritized an opportunity, the next step is generating potential solutions. The goal is not to find the one right answer immediately — it is to create a set of meaningfully different options, compare them rigorously, and select the most promising one to test. This guide covers reframing techniques, divergent and convergent thinking, evaluation methods, and strategies for avoiding cognitive biases that derail solution quality.

## From Opportunity to Solution Space: How Might We

The bridge between an opportunity and a set of solutions is the "How Might We" (HMW) question. An HMW reframes a customer need as a design challenge that invites creative exploration.

### Writing Effective HMW Statements

Take an opportunity statement and convert it into a question:

| Opportunity | HMW Question |
|------------|-------------|
| New users cannot connect their existing tools because integration setup requires technical knowledge | How might we enable non-technical users to connect their tools without needing developer help? |
| Sales managers spend hours manually consolidating pipeline data from multiple sources | How might we give sales managers a consolidated pipeline view without manual data entry? |
| Support agents do not know if a teammate has already responded to a customer | How might we make teammate activity on a ticket visible in real time? |

### HMW Calibration

The scope of your HMW question determines the breadth of solutions you will generate. Too broad and you get vague ideas. Too narrow and you constrain yourself to incremental improvements.

| HMW Scope | Example | Problem |
|-----------|---------|---------|
| **Too broad** | "How might we make onboarding better?" | Every idea qualifies. No focus. |
| **Too narrow** | "How might we add a tooltip to the integration setup page?" | This is already a solution, not a question. |
| **Right scope** | "How might we help new users complete their first integration within 5 minutes?" | Focused enough to evaluate ideas against, broad enough to allow multiple approaches. |

### HMW Variations

When a single HMW is not generating enough ideas, use these reframing techniques to open new angles:

- **Remove a constraint:** "How might we eliminate the need for integration setup entirely?"
- **Flip an assumption:** "How might we make integration errors a positive learning experience?"
- **Change the actor:** "How might we enable the customer success team to set up integrations on behalf of users?"
- **Change the timing:** "How might we set up integrations before the user even signs up?"
- **Amplify a positive:** "How might we make users who successfully connect an integration help others do the same?"
- **Explore an extreme:** "How might we guarantee 100% of users complete integration in under 60 seconds?"

Each variation generates a different solution space. Use 2-3 variations per opportunity to ensure you explore broadly before converging.

## Divergent vs. Convergent Thinking

Solution generation requires two distinct cognitive modes. Mixing them is the most common reason teams default to their first idea.

### Divergent Thinking (Expand)

The goal is quantity and variety. Generate as many ideas as possible without evaluating them.

**When to use:** At the start of solution generation, after writing your HMW questions, and whenever the team feels stuck on a single direction.

**Rules:**
- No criticism, no "yes, but..." responses
- Build on each other's ideas ("yes, and...")
- Aim for at least 10-15 ideas per HMW question
- Welcome wild ideas — they often contain seeds of practical innovation
- Set a time constraint (10-15 minutes) to maintain energy

**Techniques for divergent thinking:**

| Technique | How It Works |
|-----------|-------------|
| **Brainwriting** | Each person writes ideas silently for 5 minutes, then shares. Prevents groupthink and anchoring to the first idea spoken aloud. |
| **Analogies** | "How does [another industry] solve a similar problem?" Looking at healthcare scheduling, airline boarding, or grocery checkout can surface approaches your industry has not tried. |
| **Worst idea first** | Deliberately generate terrible solutions. Then flip them: what is the opposite of the worst idea? This loosens creative constraints. |
| **Constraint removal** | "If we had unlimited engineering time / no technical debt / a magic wand, what would we build?" Remove constraints temporarily to expand the space. |
| **Experience mining** | Each team member shares a time they encountered a similar problem in their personal life. How was it solved there? |

### Convergent Thinking (Focus)

The goal is to evaluate, filter, and select the most promising ideas.

**When to use:** After divergent thinking has produced a sufficient pool of ideas. Never during divergent thinking.

**Rules:**
- Apply explicit evaluation criteria (connected to your product outcome)
- Be willing to combine ideas — the best solution is often a hybrid
- Narrow to exactly 3 options for detailed comparison (explained below)
- Make decisions based on evidence and testability, not seniority or volume of argument

### The Rhythm

A typical solution generation session alternates:

1. **Diverge** (15 min): Generate ideas from HMW questions
2. **Cluster** (5 min): Group similar ideas into themes
3. **Diverge again** (10 min): Use reframing techniques on the most interesting clusters
4. **Converge** (15 min): Evaluate and select 3 solutions for comparison

## The Three-Solution Rule

Teresa Torres advocates always comparing at least three solutions for any given opportunity. This is not a suggestion — it is a discipline that directly improves decision quality.

### Why Three?

- **One solution means no choice.** You build whatever you thought of first. There is no comparison, no trade-off analysis, no reason to believe this is the best option.
- **Two solutions create a false binary.** Teams default to arguing for their preferred option. The debate becomes adversarial rather than analytical.
- **Three solutions force genuine comparison.** With three meaningfully different options, the team must articulate why each might or might not work. This surfaces assumptions, reveals trade-offs, and often leads to a fourth hybrid option that combines the best elements of all three.

### What "Meaningfully Different" Means

Three variations of the same idea do not count. The solutions should differ in at least one significant dimension:

| Dimension | Solution A | Solution B | Solution C |
|-----------|-----------|-----------|-----------|
| **Mechanism** | Automated setup wizard | Self-serve template library | White-glove onboarding by CS team |
| **User effort** | Very low (automated) | Medium (choose and customize) | Zero (someone does it for you) |
| **Scalability** | High | High | Low |
| **Time to value** | Minutes | 30 minutes | 1-2 days |
| **Learning for team** | High (tests automation) | Medium (tests content) | Low (tests concierge model) |

All three address the same opportunity (non-technical users cannot complete integration setup) but through fundamentally different approaches.

## Compare-and-Contrast Evaluation

Once you have three solutions, evaluate them systematically using a compare-and-contrast matrix.

### Evaluation Criteria

Choose 4-6 criteria relevant to your context. Common criteria include:

| Criterion | What It Measures |
|-----------|-----------------|
| **Outcome impact** | How directly and strongly does this solution drive the product outcome? |
| **Customer value** | How much does this reduce customer pain or increase customer capability? |
| **Reach** | What percentage of the target segment will this solution affect? |
| **Confidence** | How confident are we that this will work, given what we know? |
| **Effort** | How much engineering, design, and operational effort is required? |
| **Testability** | How quickly and cheaply can we test our riskiest assumption about this solution? |
| **Reversibility** | If this does not work, how easily can we undo it or pivot? |

### Evaluation Matrix Example

Opportunity: Non-technical users cannot complete integration setup.

| Criterion | A: Automated Wizard | B: Template Library | C: CS White-Glove |
|-----------|:---:|:---:|:---:|
| Outcome impact | High | Medium | High |
| Customer value | High | Medium | Very high |
| Reach | All new users | All new users | Enterprise only (capacity constraint) |
| Confidence | Medium — need to test if wizard handles edge cases | Medium — need to test if templates match user needs | High — manual process is proven |
| Effort | High (3-4 sprints) | Medium (1-2 sprints) | Low (hire/train CS reps) |
| Testability | Medium — prototype needed | High — can test with mock templates | High — can test with 10 customers this week |
| Reversibility | Medium — significant code to maintain or remove | High — templates easy to update or replace | High — stop offering the service |

### Using the Matrix

The matrix is a discussion tool, not a decision algorithm. Do not simply add up scores. Instead:

1. **Identify trade-offs.** Solution C has the highest customer value but the lowest reach. Is that acceptable for a first iteration?
2. **Surface assumptions.** Solution A's outcome impact is rated "high" — but that assumes the wizard handles edge cases well. Is that assumption tested?
3. **Consider sequencing.** Could you start with C (low effort, fast learning) while building toward A (high effort, high reach)?
4. **Look for hybrids.** Could you combine B's template approach with A's automation to create a template-driven wizard?

## Solution Combination Strategies

The best solution often emerges from combining elements of multiple candidates.

### Strategy 1: Best-of-Breed Combination

Take the strongest element from each solution and combine them.

Example: From the integration setup scenario:
- From Solution A: Automated detection of which tools the user needs to connect
- From Solution B: Pre-built configuration templates for common tool combinations
- From Solution C: Real-time human support available if the user gets stuck

Combined solution: An automated wizard that detects the user's tools, applies pre-built templates, and offers live chat support as a fallback. Lower cost than full white-glove, higher success rate than pure automation.

### Strategy 2: Progressive Rollout

Implement solutions as a sequence rather than choosing one.

Example:
- Week 1: Launch Solution C (CS white-glove) for the next 20 signups to learn what the biggest blockers are
- Week 4: Use those learnings to build Solution B (templates targeting the most common blockers)
- Week 8: If templates work, invest in Solution A (full automation) with confidence

### Strategy 3: Segment-Based Combination

Use different solutions for different customer segments.

Example:
- Enterprise accounts: Solution C (white-glove) — high-touch matches their expectations
- Mid-market accounts: Solution B (templates) — self-serve with guided content
- SMB accounts: Solution A (automated wizard) — fully automated for scale

## Avoiding First-Idea Bias and Anchoring

Cognitive biases consistently push teams toward building the first solution someone suggests. Awareness alone does not fix this — you need structural countermeasures.

### First-Idea Bias

**What it is:** The tendency to anchor on the first solution proposed and evaluate all subsequent ideas relative to it. The first idea becomes the default; alternatives must "prove" they are better.

**Why it happens:** The first idea occupies mental space. It feels concrete and familiar. Alternatives feel abstract and risky by comparison. Additionally, if the first idea comes from the most senior person in the room, social dynamics amplify the bias.

**Countermeasures:**

| Countermeasure | How It Works |
|---------------|-------------|
| **Silent ideation first** | Everyone writes ideas independently before any discussion. This prevents the first speaker from anchoring the group. |
| **Require three before discussing any** | Do not evaluate any idea until at least three are on the table. This normalizes comparison. |
| **Devil's advocate rotation** | Assign someone to argue against the leading idea. Rotate the role so it is not personal. |
| **Sleep on it** | If possible, generate ideas in one session and evaluate in another. Distance reduces anchoring. |

### Sunk Cost Anchoring

**What it is:** Favoring a solution because work has already been done on something similar. "We already built half of this" becomes a reason to continue even when a better option exists.

**Countermeasure:** Evaluate solutions as if starting from scratch. Ask: "If we had not built anything yet, would we choose this approach?" If the answer is no, the sunk cost is misleading you.

### Confirmation Bias in Evaluation

**What it is:** Seeking evidence that supports the preferred solution and ignoring evidence against it.

**Countermeasure:** For each solution, explicitly list the assumptions that must be true for it to work. Then ask: "What evidence would make us abandon this solution?" Define the failure criteria before testing.

### Authority Bias

**What it is:** Deferring to the highest-ranking person's preferred solution regardless of evidence.

**Countermeasure:** Use the product trio structure (PM, designer, tech lead) as equal decision-makers. Collect input through brainwriting before discussion. Make decisions based on the evaluation matrix, not hierarchy.

## Worked Example: Three-Solution Comparison

**Product outcome:** Increase the percentage of free trial users who invite a second team member from 12% to 25%.

**Target opportunity:** Users do not see the value of inviting teammates because the product feels like a single-player tool during the trial.

**HMW:** How might we help trial users experience the collaborative value of the product before inviting anyone?

### Solution A: Simulated Collaboration

Show the user what the product looks like with teammates by populating their workspace with simulated activity — sample comments, shared dashboards, and notifications from fictional teammates. The user sees what collaboration feels like and is motivated to invite real people.

### Solution B: Shared Trial Workspace

Instead of each trial user getting an isolated workspace, pair new signups into small cohort workspaces (3-5 strangers in the same trial group). They experience real collaboration with real people from day one.

### Solution C: Invite-Gated Feature

Identify the single most compelling collaborative feature (e.g., shared dashboards). Make it visible but locked behind inviting one teammate. The user sees a preview, understands the value, and invites someone to unlock it.

### Comparison

| Criterion | A: Simulated | B: Cohort Workspace | C: Invite-Gated |
|-----------|:---:|:---:|:---:|
| Outcome impact | Medium — simulation may not transfer to real behavior | High — real collaboration creates real motivation | High — direct mechanism to drive invites |
| Customer value | Medium — useful for preview but feels artificial | High — genuine value from day one | Medium — value gated behind action |
| Risk | Users may find simulated activity misleading or annoying | Privacy concerns; strangers in shared workspace | Users may feel manipulated; churn risk if feature feels locked |
| Effort | Medium (2 sprints) | High (3-4 sprints, operational complexity) | Low (1 sprint) |
| Testability | Medium — prototype test possible | Low — need real users in real cohorts | High — can A/B test in one week |
| Key assumption | Users will connect simulated value to real-teammate value | Strangers will meaningfully interact in a trial workspace | The gated feature is compelling enough to drive invites |

### Decision

The team might choose to test Solution C first (lowest effort, highest testability, directly drives the metric), use learnings to refine their understanding of which collaborative features matter most, and then consider Solution A or a hybrid for the next iteration.

## When to Stop Generating and Start Testing

Solution generation should be timeboxed. Teams that keep generating ideas indefinitely are often avoiding the discomfort of committing to a direction.

**Stop generating when:**
- You have at least three meaningfully different solutions
- You can articulate the riskiest assumption for each
- The team can clearly state why each solution might or might not work
- You have spent no more than 1-2 sessions (2-4 hours total) on ideation and evaluation

**Start testing when:**
- You have selected one solution (or a hybrid) based on the compare-and-contrast evaluation
- You have identified the riskiest assumption that must be true for the solution to work
- You can design a small, fast experiment to test that assumption

The value of solution generation is not in finding the perfect answer. It is in exploring the space broadly enough that you have confidence your selected direction is strong relative to the alternatives. Perfection comes from iteration, not from longer brainstorming sessions.

## Summary

Effective solution generation follows a clear sequence: reframe the opportunity as an HMW question, diverge to create many options, converge to select three meaningfully different solutions, compare them using explicit criteria, look for hybrid combinations, and select the one with the best balance of impact and testability. The three-solution rule, silent ideation, and structured evaluation matrices are not optional refinements — they are the structural countermeasures that prevent teams from defaulting to the first idea and calling it a strategy.
