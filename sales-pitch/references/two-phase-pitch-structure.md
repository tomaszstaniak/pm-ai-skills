# Two-Phase Pitch Structure

The two-phase structure — Setup followed by Follow-Through — is the architectural foundation of every effective sales conversation. This reference covers all eight components in depth, with worked examples, timing guidance, component-level templates, and diagnostic tools for the most common failure modes in B2B software pitches.

## Why the Sequence Cannot Be Reversed

The Setup doesn't just provide background — it constructs the cognitive framework through which buyers will evaluate everything in the Follow-Through. Without it, your differentiation arrives before the buyer has any basis for judging it against alternatives. Feature claims land as marketing copy. Value statements feel abstract. The buyer has no way to distinguish "we're faster" from every competitor who says the same thing.

With a completed Setup, the same statement lands differently: the buyer has already internalized what alternatives exist, what trade-offs each carries, and what an ideal solution would look like for their situation. Your Follow-Through now reads as the logical conclusion of a market analysis — one the buyer participated in. That shift is the entire mechanism.

**The rule:** Do not move from Setup to Follow-Through until the buyer has confirmed alignment. Explicit confirmation. Not nodding, not polite silence — the buyer should be able to summarize the market dynamics and their own requirements back to you.

---

## Phase One: Setup

### Component 1 — Market Insight

**Purpose:** Establish credibility as a market expert, not a sales rep. Shift the buyer's posture from guarded to curious.

**What it is:** A specific, experience-grounded observation about the problem space that demonstrates you've seen this situation across many companies — and have learned something from that exposure that the buyer probably hasn't fully articulated yet.

**What it is not:** A generic industry trend, a statistic from an analyst report, or a claim designed to manufacture urgency.

**Timing:** 60 seconds for experienced buyers in a familiar category. 3–4 minutes with discovery questions woven in for buyers new to the category or in complex environments.

**Template:**

| Element | Description | Example |
|--------|-------------|---------|
| Pattern observed | The recurring situation you've seen across customers | "Most engineering teams we work with…" |
| The turning point | The moment the current approach breaks down | "…hit a wall when their release cycle drops below two weeks…" |
| Why it matters | The consequence of that breakdown | "…because their existing monitoring setup can't distinguish signal from noise at that frequency." |
| Relevance check | Confirm this applies to the buyer | "Is that consistent with what you're running into?" |

**Worked examples by context:**

*DevOps platform, mid-market engineering team:*
> "One thing we see consistently in engineering orgs of your size — usually somewhere between 40 and 80 engineers — is that incident response works fine until on-call rotation expands past two or three people. At that point, alert routing that used to be informal starts requiring policy, and the tools that handled informal don't have the configuration depth for policy. Teams either build that layer themselves or start losing engineers to burnout. Does that pattern show up for you?"

*Data analytics SaaS, VP of Data Science:*
> "The analytic teams we work with most often come to us right after a business intelligence tool rollout that didn't get the adoption the data team expected. The BI tool is solid — that's rarely the problem. What's almost always the problem is that the underlying data model wasn't designed for business users to navigate independently. The tool assumes data literacy the business doesn't have. When did you ship your current BI setup?"

*Enterprise HR software, CHROs at companies post-acquisition:*
> "The companies we talk to after an acquisition almost always have the same HRIS problem: two systems with different employee taxonomies, and no clean way to run cross-entity reporting during the integration period. Finance needs headcount data the HR system can't produce at the granularity they want. That usually surfaces about 90 days post-close. Where are you in that timeline?"

**Weak vs. strong insights by context:**

| Context | Weak Insight | Strong Insight |
|---------|-------------|----------------|
| SaaS analytics tool | "Companies are drowning in data." | "Most analytics teams we work with hit a wall when data requests from the business start outnumbering analyst capacity — usually around 3:1. At that point, self-serve tools get deployed but adoption stays under 20% because the underlying data model isn't business-user-ready." |
| DevSecOps platform | "Security is more important than ever." | "The pattern we see in engineering orgs that ship fast is that security debt accumulates in the same three places every time: dependency management, secrets handling, and access reviews. The first two are automatable; the third almost always requires a manual process that nobody owns." |
| Enterprise HR software | "Talent retention is a challenge." | "The companies coming to us after failed HRIS implementations share one thing: their previous vendor scoped the project around HR users, not managers. Manager adoption predicts whether the system actually changes behavior — and it's almost never in the implementation plan." |

**Copy patterns:**
- "Before I show you what we do, I want to share what we've learned working with companies like yours in this space…"
- "One thing we've learned working with [similar companies] is that…"
- "The pattern we see consistently in this space is…"
- "What surprises most of our customers when they first talk to us is…"

**Quality check:** If the buyer responds with "yes, exactly" or a story that confirms your observation — you have a strong insight. If they look uncertain or give a polite non-response, your insight wasn't specific enough to be recognizable.

---

### Component 2 — Alternatives

**Purpose:** Show the buyer a complete, honest map of their options. Establish yourself as a trusted guide rather than an advocate for a predetermined conclusion.

**What it is:** A structured walk through the realistic approaches a buyer in this situation would consider — including the option to do nothing.

**What it is not:** A competitive teardown. A rigged comparison. A slide where your product is the obvious winner before any criteria are discussed.

**Timing:** 3–8 minutes depending on category complexity and how many genuine alternatives exist.

**Template:**

| Alternative | Honest strength | Honest trade-off | Best fit for |
|------------|-----------------|-----------------|--------------|
| Competitor A | Where they genuinely lead | Where their approach creates friction | Buyer profile where they win legitimately |
| Adjacent solution | Appeal — usually cost or control | Hidden costs or capability gaps | Simpler use cases where full solution is overkill |
| Build in-house | Maximum customization, no vendor dependency | Ongoing maintenance, opportunity cost, time to value | Orgs with specific regulatory or integration requirements that commercial products can't meet |
| Do nothing / status quo | Known, stable, no migration risk | The specific, compounding cost of staying here | No one — frame this as an active choice, not a neutral default |

See [competitive-alternatives-framing.md](competitive-alternatives-framing.md) for depth: the four-alternative-type taxonomy, handling "do nothing" as your fiercest competitor, honest-strength-then-trade-off framing, and the anti-patterns that destroy credibility.

---

### Component 3 — Perfect World

**Purpose:** Help the buyer articulate what an ideal solution looks like for their specific situation — before you introduce your product.

**What it is:** A collaborative definition of the evaluation criteria that would make a solution genuinely right for this buyer, given what you've just walked through together.

**What it is not:** A feature list of your product. A leading question designed to get the buyer to name your differentiators without realizing it.

**Timing:** 2–4 minutes, primarily discovery-driven. This is a listening exercise, not a presentation.

**How to execute:**

1. Transition from the alternatives summary: *"Given what we just walked through — the trade-offs of each approach — if you could design the ideal solution for your situation, what would it need to do?"*
2. Listen without interrupting. Let the buyer name criteria.
3. Add any criteria your experience tells you matter that the buyer hasn't mentioned: *"One thing I'd add that comes up consistently for companies in your situation is [criteria]. Is that relevant here?"*
4. Reflect back and confirm: *"So it sounds like the ideal solution would need to [X, Y, Z], and probably not require [constraint they named]. Is that a fair summary?"*

**The completion signal:** The Setup is finished when the buyer confirms a summary of (a) the market dynamics, (b) the trade-offs of alternatives, and (c) what they'd need in an ideal solution. All three. If you move to Follow-Through without this, you're guessing at relevance.

---

## Phase Two: Follow-Through

### Component 4 — Introduction

**Purpose:** Place your product in the landscape the buyer now understands. Answer the question "where do you fit?" in the context of the map you just drew together.

**What it is:** A precise, confident statement of what you are and where you sit — grounded in the alternatives discussion the buyer just had with you.

**Timing:** 30–60 seconds. This is a placement, not a pitch.

**Template:**
> "Given what we've just walked through, here's where [Product] fits. We're a [category] built specifically for [best-fit customer type]. The way to think about us relative to the options we just discussed is [positioning relative to alternatives]. The reason companies in your position typically come to us — rather than [alternative] — is [the specific gap your product fills that the landscape discussion surfaced]."

**Worked example (security platform, mid-market):**
> "So where Vanta fits in the map we just drew: we're a trust management platform built specifically for mid-market software companies that need to move through compliance frameworks — SOC 2, ISO, HIPAA — without pulling engineering off product work to do it. Relative to what we discussed: we're not the right answer for companies that want to build their GRC program in a spreadsheet, and we're not the enterprise GRC platform your compliance team would buy if you had 500 engineers and a dedicated InfoSec team. We're the path between those options — automated evidence collection, continuous monitoring, and auditor-ready reporting for teams that want compliance without a compliance department."

---

### Component 5 — Differentiated Value

**Purpose:** State the specific business outcomes only you can deliver, in the context of the alternatives the buyer already understands.

**Timing:** The core of the Follow-Through — typically 5–10 minutes in a discovery meeting, tightened to a single deeply substantiated claim for executive audiences.

**Template:** Every claim should be comparative and outcome-based — "Unlike [alternative], which [limitation], our [capability] means [business outcome the buyer's CFO would care about]."

**Worked example — developer tooling, head of platform engineering:**
> "The thing we do that's genuinely different from what you'd get with [Competitor X] is our policy-as-code layer. In their model, security policies live in the platform UI and get manually maintained by your security team. In ours, policies are versioned in your repository alongside the code they govern. The practical consequence: your security posture is auditable the same way your code is auditable, and your platform team doesn't have to chase policy drift across environments. For an org running twelve microservices with separate deployment pipelines, that's the difference between a security review that takes a week and one that takes an afternoon."

See [differentiated-value-development.md](differentiated-value-development.md) for depth: the "so what / compared to what" two-question test, worksheets for turning capabilities into claims, and how to identify and cut weak claims.

---

### Component 6 — Proof

**Purpose:** Reduce the buyer's perceived risk by showing that your claims hold in situations that look like theirs.

**Proof selection matrix** — match proof format to the buyer's profile and evaluation stage:

| Buyer profile / stage | Best proof format | Caution |
|--------------|-----------------|---------|
| Early in evaluation, unfamiliar with category | Market data, peer benchmarks, analyst validation | Don't lead with case studies that assume category literacy |
| Mid-evaluation, comparing options | Customer case study matched by industry, size, and use case | Mismatched case studies raise doubt rather than confidence |
| Late-stage, technical evaluation in progress | Live demo proving specific differentiation claims, plus reference calls | Demo must prove the specific thing you claimed — a feature tour is not proof; choose references who match the buyer's situation and prepare them for likely questions |
| Executive sponsor, risk-focused | Quantified outcome data with defensible methodology, named customer willing to speak | Unverifiable numbers are worse than no numbers; aggregate figures without context feel fabricated |
| Champion building internal case | One-page evidence summary they can share without you in the room | Must be self-explanatory and not require your narration to make sense |
| Buyer distrusts vendor-produced evidence (any stage) | Third-party validation — analyst coverage, review site ratings, independent benchmarks | Carries credibility vendor content can't, but only if genuinely independent |

**Proof statement template:**
> "Let me show you what this actually looked like for [company type that matches the buyer]. They were in a similar situation — [brief framing that mirrors the buyer's context]. Here's what they were dealing with: [the problem]. Here's what changed after implementation: [specific, quantified outcome]. And here's the part that's directly relevant to [the specific concern raised in this conversation]: [the piece of evidence that addresses that concern specifically]."

**Copy patterns:**
- "I want to show you exactly the thing I claimed we do differently, in the actual product, so you can see how it works rather than just take my word for it…"
- "The number I keep hearing from customers in your segment is [specific metric] — here's where that comes from and why it's typical for your type of deployment…"

---

### Component 7 — Objection Handling

**Purpose:** Address anticipated concerns proactively, before they become late-stage blockers.

**The key shift:** Objections handled proactively in the pitch read as confidence and transparency. Objections surfaced for the first time during procurement or legal review read as things you were hoping to avoid.

**Proactive handling formula:**
> "One question that comes up for almost every company in your situation is [objection]. The honest answer is [direct response that acknowledges any legitimate basis for the concern, then addresses it]. Here's how other customers have navigated that: [specific evidence or approach]."

**Common objection types in B2B software:**

| Objection type | How to surface proactively | What not to do |
|---------------|---------------------------|----------------|
| Migration / implementation risk | "I want to address something we see as a common concern at this stage: migration from [current system]…" | Minimize the concern; buyers who discover later you underplayed it will walk |
| Vendor stability / longevity | For early-stage companies: address funding, customer retention, and roadmap transparency directly | Deflect with vague confidence; buyers will research independently |
| Pricing vs. alternatives | Frame total cost of ownership, not just license cost | Compete on price alone; you'll lose on price alone |
| Integration with current stack | Specifically address the two or three integrations most relevant to this buyer | Generic "we integrate with everything" claims; list specific, tested integrations |
| Internal adoption / change management | Reference how comparable customers handled rollout; offer support for it | Promise results without addressing the behavior change required to get them |

---

### Component 8 — The Ask

**Purpose:** Create a specific, friction-free path to the next step.

**What "friction-free" means:** The ask is sized appropriately for the stage of the relationship and the complexity of the decision. Asking for a signed contract after a first meeting is high friction. Asking to schedule a two-hour technical deep-dive after a 20-minute intro call is high friction. The right ask moves the deal forward without requiring a commitment the buyer isn't ready to make.

**The three elements of a strong ask:**
1. **Specific action** — not "let's stay in touch" or "let me follow up"
2. **Clear outcome** — what will the buyer know or have after the next step?
3. **Named timeline** — a date, not "sometime soon"

**Ask templates by deal stage:**

| Stage | Weak ask | Strong ask |
|-------|----------|-----------|
| First conversation | "I'll send over some material." | "Can we get 45 minutes on the calendar with your technical lead? I want to show them specifically how the integration with [their current tool] works — that's usually the question that determines fit at the next stage. How's [specific date]?" |
| Post-demo | "Let us know if you have questions." | "The next step I'd suggest is a reference call with [similar company] — they were in the exact situation you described. If that conversation confirms what you're seeing, we'd move to a scoping session. Want me to set that up for next week?" |
| Technical evaluation | "We can extend the trial." | "You've got two weeks left in the POC. Let's set a checkpoint on [date] to review what the data is showing — I'll have [technical contact] from our side on the call. That gives us time to address anything before the evaluation closes." |
| Final stage | "Take the time you need." | "Based on our last conversation, the two things you wanted to confirm were [X and Y]. I've addressed both in the proposal. If those hold, what does your internal process look like from here, and who do I need to make sure has what they need?" |

---

## Complete Pitch Structure Diagnostic

Run this check before any significant pitch — new prospect, new audience, or a revision to an existing deck.

| Component | Diagnostic question | If no | Fix |
|-----------|-------------------|-------|-----|
| Market Insight | Is the insight specific enough that a buyer could only have heard it from someone who has worked closely with their type of company? | Generic insight | Replace with a pattern observed across 10+ real customer situations |
| Alternatives | Does the alternatives tour include the competitor you most fear, characterized honestly? | Competitor omitted or misrepresented | Add them; acknowledge their genuine strengths first |
| Alternatives | Is "do nothing" included as a named option with specific costs? | Inaction unaddressed | Add a quantified cost-of-status-quo statement |
| Perfect World | Does the Setup end with a buyer-confirmed summary of their ideal criteria? | No confirmation | Add explicit check: "Does that feel like an accurate summary of what you'd need?" |
| Introduction | Is product placement grounded in the map from the Setup? | Introduction feels disconnected | Rewrite using language from the alternatives discussion |
| Differentiated Value | Do all value claims pass both "so what?" and "compared to what?" | Vague or generic claims | Run the two-test filter on every claim; cut any that fail |
| Proof | Is proof selected to match this buyer's industry, size, and use case? | Generic logo wall or mismatched case studies | Build a proof library segmented by buyer profile; select accordingly |
| Objections | Are the top three anticipated concerns addressed proactively? | Objections surface late as surprises | Run a pre-pitch objection mapping exercise with your team |
| The Ask | Does the ask name a specific action, outcome, and date? | Vague "follow up" | Script the ask before the meeting; deliver it at the close |

---

## Timing Reference by Format

| Format | Setup target | Follow-Through target | Notes |
|--------|-------------|----------------------|-------|
| Cold outbound call (15 min) | 90 seconds | 5–6 minutes; lead with sharpest differentiator | Cut to one insight, one alternative contrast, one value claim |
| First discovery meeting (45–60 min) | 15–20 minutes with discovery woven in | 15–20 minutes tailored to pain uncovered | Discovery questions belong inside the Setup, not before it |
| Demo to technical evaluators (60 min) | 10 minutes emphasizing architecture trade-offs | 35–40 minutes; proof-heavy with live demonstration | Demo should prove specific differentiation claims, not tour features |
| Executive sponsor meeting (30 min) | 8–10 minutes; focus on business outcomes and risk | 15 minutes; ROI-forward, risk-addressed | One differentiated value claim, deeply substantiated |
| Written proposal | Setup summarized in 1–2 paragraph context section | Main body: value, proof, next steps | Setup sets the evaluation frame so Follow-Through reads as the logical answer |
| Conference talk or webinar | Full Setup as the main act (teaches the problem) | 5–10 minutes at the end introducing your approach | The audience is a cold prospect; don't pitch until you've earned it |

---

The two-phase structure isn't a presentation format — it's a discipline about sequencing. The Setup earns the right to be heard. The Follow-Through converts that attention into a decision. When both phases are present and complete, deals close on merit. When either is rushed or skipped, the structure breaks down and outcomes become unpredictable. Every component in this reference exists to make one of those two phases work properly — use them in that context.