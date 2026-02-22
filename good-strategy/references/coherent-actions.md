# Coherent Actions: Building an Activity System That Reinforces Itself

Strategy is not a collection of independent initiatives. It is a set of actions that work together. The power of good strategy comes from coherence — actions that reinforce each other, creating a system that is worth more than the sum of its parts and that is difficult for competitors to replicate. This guide covers how to design, map, and audit action coherence using Porter's framework of activity fit and Rumelt's emphasis on coordinated action.

## Porter's Three Levels of Activity Fit

Michael Porter identifies three levels of fit among a company's activities. Each level increases the strategic power and defensibility of the system.

### Level 1: Simple Consistency

Each activity is aligned with the overall guiding policy. No activity contradicts the strategy.

**What it looks like:** If your guiding policy is "compete on speed of deployment," then your hiring practices, tooling choices, release processes, and customer support model all support speed. Nothing actively works against it.

**What it does not do:** Simple consistency prevents self-sabotage, but it does not yet create compounding advantage. Each activity could theoretically be copied independently.

**Test:** For each major activity, ask: "Does this support or contradict our guiding policy?" If any activity contradicts it, you have an inconsistency to resolve.

| Activity | Supports Policy? | Contradicts Policy? | Neutral? |
|----------|-------------------|---------------------|----------|
| Engineering practices | | | |
| Hiring criteria | | | |
| Sales process | | | |
| Customer support model | | | |
| Pricing structure | | | |
| Marketing approach | | | |
| Partner relationships | | | |

### Level 2: Reinforcing Activities

Activities do not merely align with the strategy — they amplify each other. The value of Activity A increases because Activity B exists, and vice versa.

**What it looks like:** A company that competes on developer experience invests in excellent documentation (Activity A) and a community forum (Activity B). The documentation reduces support burden, freeing engineering time to improve the product. The community forum generates content that supplements the documentation. Better documentation drives more community participation. Each activity makes the other more effective.

**What it does not do:** Reinforcing activities are more powerful than simple consistency, but they can still be partially replicated if a competitor is willing to invest in the same combination.

**Test:** For each pair of major activities, ask: "Does Activity A make Activity B more effective, and does Activity B make Activity A more effective?" Look for mutual reinforcement, not just co-existence.

**Reinforcement matrix example:**

| | Docs | Community | API Design | Support |
|---|---|---|---|---|
| **Docs** | — | Docs seed forum answers; forum surfaces doc gaps | Good API needs less docs; docs showcase API patterns | Docs reduce ticket volume |
| **Community** | Forum supplements docs | — | Community feedback shapes API | Community handles L1 questions |
| **API Design** | Clean API = simpler docs | Intuitive API = happier community | — | Clean API = fewer support issues |
| **Support** | Support identifies doc needs | Support redirects to community | Support logs shape API priorities | — |

### Level 3: Optimization of Effort

Activities are designed together as a system where trade-offs are made at the system level, not the activity level. Changing one activity would degrade the performance of many others.

**What it looks like:** IKEA's activity system is the classic example. Flat-pack furniture (Activity A) enables self-service warehouses (Activity B), which enable lower prices (Activity C), which attract cost-conscious customers who are willing to self-assemble (Activity D), which validates the flat-pack design choice (back to A). Changing any single element — say, switching to assembled furniture — would break the warehouse model, raise prices, change the customer base, and unravel the entire system.

**What makes it defensible:** A competitor cannot replicate one or two activities and get the same result. The advantage comes from the system, not from any individual piece. To compete, a rival would need to replicate the entire system simultaneously — which is extremely difficult.

**Test:** Pick any single activity and ask: "If we changed or removed this, how many other activities would need to change?" If the answer is "most of them," you have system-level optimization.

## How to Create an Activity System Map

An activity system map visualizes the relationships between your organization's major activities and reveals where reinforcement exists (or is missing).

### Step 1: List Core Activities

Identify 8-15 activities that are central to how your organization creates and delivers value. These should be activities, not departments. Focus on what is done, not who does it.

Examples for a product-led growth SaaS company:
- Free tier with generous limits
- Self-serve onboarding (no sales required)
- In-product upgrade prompts based on usage
- Usage-based pricing
- Community-driven support
- Public API with extensive documentation
- Automated provisioning and deployment
- Product analytics driving roadmap
- Content marketing focused on tutorials

### Step 2: Map Reinforcement Links

For each pair of activities, ask whether they reinforce each other. Draw a link between activities that mutually reinforce. Use different line weights or styles to indicate strength of reinforcement.

A strong reinforcement link means: removing Activity A would measurably reduce the effectiveness of Activity B.

A weak reinforcement link means: Activity A supports Activity B, but Activity B would function nearly as well without it.

### Step 3: Identify the Hub Activities

Hub activities have the most reinforcement links. These are the activities that, if changed, would affect the most other activities. Hub activities are the hardest to change and the most strategically important to protect.

In the IKEA example, flat-pack design is a hub activity. In a product-led growth company, the free tier and self-serve onboarding are hub activities.

### Step 4: Identify Orphan Activities

Orphan activities have few or no reinforcement links. They may be legacy initiatives, pet projects, or responses to one-time competitive threats. Orphan activities consume resources without contributing to the strategic system. They are candidates for elimination or redesign.

### Step 5: Identify Missing Links

Look for activities that should reinforce each other but don't. These are opportunities to strengthen the system. Often the fix is not adding a new activity but redesigning an existing one to create reinforcement.

## Coherence Audits: Testing Your Action System

A coherence audit evaluates whether your organization's actions reinforce each other or pull in different directions.

### The Contradiction Scan

List your top five strategic initiatives. For each pair, ask: do these initiatives compete for the same resources? Do they send conflicting signals to the organization? Do they require incompatible capabilities?

| Initiative A | Initiative B | Contradiction? | Nature of Conflict |
|-------------|-------------|----------------|-------------------|
| | | | |

Common contradictions:

- **Speed vs. quality:** "Ship faster" and "reduce defect rate" may require different engineering practices, testing investments, and risk tolerances.
- **Growth vs. profitability:** "Acquire more customers" and "improve unit economics" may conflict when customer acquisition costs are high.
- **Innovation vs. reliability:** "Experiment more" and "maintain platform stability" require different technical architectures and team cultures.

The presence of a contradiction does not always mean one initiative is wrong. Sometimes it means the guiding policy needs to resolve the tension by specifying which side wins when they conflict.

### The Resource Allocation Test

Rumelt and others observe that the real strategy of an organization is revealed by where it spends money and allocates people — not by what its strategy document says.

Perform this audit:

1. List your stated strategic priorities (from the guiding policy).
2. List where your top 20 engineers spend their time.
3. List your top 10 budget line items.
4. Compare.

| Stated Priority | % of Engineering Time | % of Budget | Aligned? |
|-----------------|----------------------|-------------|----------|
| | | | |
| | | | |
| | | | |

If a stated priority receives less than 15% of relevant resources, it is not a real priority. If something that is not a stated priority receives more than 20% of resources, the actual strategy differs from the stated strategy.

This gap between stated and actual strategy is one of the most common sources of incoherence. Closing it requires either changing the stated strategy to match reality or reallocating resources to match the stated strategy.

### The Message Consistency Test

Ask five people in different roles: "What is our strategy?" If you get five different answers, your strategy is either unclear, incoherent, or both. The answers reveal which elements of the strategy have actually been internalized and which exist only in documents.

## How to Detect and Fix Incoherence

### Signals of Incoherence

| Signal | What It Indicates |
|--------|-------------------|
| Every team has different "priorities" | No guiding policy, or it is too vague to constrain choices |
| Resource allocation does not match stated strategy | Actual strategy differs from stated strategy |
| Initiatives frequently cancel or pivot | Lack of conviction in the diagnosis, or multiple competing diagnoses |
| Teams optimize locally at the expense of others | No system-level design; activities are independent, not reinforcing |
| Strategic reviews produce new initiatives without retiring old ones | Accumulation without coherence; strategy by accretion |
| Customers receive mixed messages | Sales promises differ from product reality because the guiding policy is ambiguous |

### The Fix Protocol

1. **Start with the diagnosis.** If the diagnosis is unclear, no amount of action-level tinkering will create coherence. Go back to the strategic diagnosis and sharpen it.
2. **Sharpen the guiding policy.** Make sure the trade-offs are explicit. If the policy doesn't rule things out, it cannot create coherence.
3. **Map the activity system.** Identify which activities reinforce the guiding policy and which contradict it.
4. **Retire contradictory activities.** This is the hardest step politically and the most important strategically. Activities accumulate over time, and each has a constituency. Removing one requires leadership willing to make explicit trade-offs.
5. **Design reinforcement.** For each remaining activity, ask: how can this be modified to better reinforce at least two other activities?
6. **Align resource allocation.** Shift resources away from orphan and contradictory activities toward hub and reinforcing activities.

## Worked Examples

### Coherent Action Set: Developer Platform

**Guiding policy:** "Win by making developers productive in the first 30 minutes."

| Activity | Reinforces | Why |
|----------|------------|-----|
| Interactive getting-started tutorial | Onboarding speed, community engagement | Developers complete the tutorial and share results |
| Opinionated CLI tooling | Onboarding speed, support cost reduction | CLI makes common tasks trivial, reducing questions |
| Free tier with no credit card | Onboarding speed, community size | Removes friction; larger community generates more content |
| Public Slack community | Support cost reduction, product feedback | Community members answer each other's questions; feature requests are visible |
| Usage-based pricing | Free tier sustainability, expansion revenue | Free tier costs are low; revenue scales with actual value delivered |

This is a coherent set: each activity supports at least two others, and all point toward the guiding policy of first-30-minutes productivity.

### Incoherent Action Set: The Same Company, Poorly Executed

| Activity | Problem |
|----------|---------|
| Interactive tutorial | Hasn't been updated in 8 months; references deprecated APIs |
| Opinionated CLI tooling | Team also maintains a GUI dashboard that requires a different mental model, splitting engineering effort |
| Free tier with no credit card | Sales team pressures product to gate features behind "book a demo," contradicting self-serve ethos |
| Public Slack community | Community is unmonitored; questions go unanswered for days, creating negative impression |
| Enterprise sales motion | Sales team pursues enterprise deals requiring custom SLAs, security reviews, and dedicated support — activities that serve a different guiding policy |

The incoherence here stems from trying to pursue two strategies simultaneously (product-led growth and enterprise sales) without resolving the tensions between them. Each strategy is individually viable, but pursuing both creates activities that undermine each other.

## Template for Mapping and Evaluating Action Coherence

### Step 1: List Your Top Strategic Actions

Write down the 8-12 most significant initiatives, investments, or operational activities currently underway or planned.

### Step 2: Build the Reinforcement Matrix

Create a matrix with all actions on both axes. For each cell, note whether the row activity reinforces (+), contradicts (-), or has no relationship (0) with the column activity.

### Step 3: Score Each Action

| Action | Links to Policy | Reinforcing Links | Contradicting Links | Net Score |
|--------|----------------|-------------------|---------------------|-----------|
| | Direct / Indirect / None | Count of + | Count of - | + minus - |

### Step 4: Classify Each Action

- **Hub actions** (high reinforcing links, direct policy link): Protect and invest
- **Supporting actions** (moderate reinforcing links): Maintain and look for reinforcement opportunities
- **Orphan actions** (few links): Evaluate whether to redesign for reinforcement or retire
- **Contradictory actions** (negative net score): Retire or fundamentally restructure

### Step 5: Design Improvements

For each orphan or contradictory action, choose one:

| Action | Decision | Rationale |
|--------|----------|-----------|
| | Retire / Redesign / Escalate | |

### Step 6: Validate Resource Allocation

Ensure that hub and supporting actions receive the majority of resources. If an orphan or contradictory action is consuming significant resources, this is the highest-priority fix.

The ultimate measure of coherence is not whether each action individually makes sense, but whether the actions collectively form a system that is greater than the sum of its parts. A set of individually reasonable actions that pull in different directions is worse than a set of individually modest actions that powerfully reinforce each other. Coherence is the multiplier that turns effort into strategic advantage.
