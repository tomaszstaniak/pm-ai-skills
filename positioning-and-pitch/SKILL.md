---
name: positioning-and-pitch
description: 'Framework based on April Dunford''s "Obviously Awesome" and "Sales Pitch". Use this skill whenever the user is discussing how to describe, frame, differentiate, sell, or talk about their product — even if they do not explicitly say "positioning," "pitch," or "messaging." Triggers include: (1) defining or evaluating product positioning using the five-component framework, (2) translating positioning into a compelling pitch for execs, boards, partners, or buyers, (3) choosing a market category strategy that shapes what you build and how you compete, (4) developing differentiated value claims, (5) diagnosing why your product story isn''t landing with customers or stakeholders, (6) aligning teams around a shared positioning narrative and connecting it to roadmap priorities, (7) writing a launch announcement, website headline, or tagline, (8) deciding which features to highlight in marketing copy, demos, or sales decks, (9) responding when a buyer says "you sound like everyone else."'
license: CC-BY-SA-4.0
metadata:
  author: Tomasz Staniak
  version: "1.0.0"
---

# Positioning and Pitch (Dunford)

This skill captures the strategic positioning framework from April Dunford's *Obviously Awesome* and the pitch construction model from *Sales Pitch*, combined into a single cohesive framework for product managers. It covers how to define where your product wins, for whom, and why — and how to translate that positioning into pitches that land with executives, boards, partners, and buyers. Positioning is not a marketing exercise. It's the upstream decision that determines what you build, who you build for, and how you talk about it.

## Core Principle

**PMs who can't articulate why their product wins in a specific market context can't make good roadmap decisions, can't align stakeholders, and can't enable sales — positioning is the strategic act that connects product decisions to market reality.**

Positioning feels like a marketing deliverable until you realize it's the decision that shapes everything downstream. Your market category determines which competitors buyers compare you to and which features they expect. Your differentiated value determines which capabilities deserve investment and which are distractions. Your best-fit customer definition determines where discovery should focus and which segments your roadmap should serve. Your pitch — to executives, to the board, to partners, to customers — is just positioning delivered in context.

Most product teams skip positioning or treat it as a one-time launch exercise. The result is predictable: roadmaps that try to serve everyone, pitches that sound like every competitor's, stakeholder conversations where the PM can't explain why this feature matters more than that one. When positioning is clear, product decisions get easier. When it's absent, every decision becomes a negotiation without shared criteria.

Dunford's framework is built on a specific insight: positioning is not messaging. It's the set of assumptions — about your competitive context, your unique strengths, and your target market — that messaging is derived from. Get the positioning wrong and no amount of wordsmithing fixes the pitch.

## Scoring

**Goal: 10/10.** When evaluating positioning and pitch quality, rate 0–10:

| Score | Description |
|-------|-------------|
| 0–2 | No explicit positioning. Product described in generic terms ("we help companies do X better"). No competitive context. Pitch is a feature walkthrough. Stakeholders can't explain what makes the product different. Roadmap has no filtering criteria — every request is equally valid. |
| 3–4 | Positioning exists informally but isn't documented or shared. Different team members describe the product differently. Market category is vague or aspirational. Differentiation claims are generic ("faster," "easier," "more flexible"). Pitch works for some audiences but confuses others. |
| 5–6 | Five positioning components are partially defined. Competitive alternatives are acknowledged but not systematically mapped. Differentiated value is articulated but hasn't passed the "so what / compared to what" test. Pitch has structure but doesn't adapt to different stakeholder contexts. Roadmap is loosely informed by positioning. |
| 7–8 | All five components are clearly defined and documented. Differentiated value is specific, comparative, and grounded in real capabilities. Best-fit customer definition actively filters discovery and roadmap decisions. Pitch adapts to context — exec reviews, board updates, sales enablement. Cross-functional team can articulate the same positioning story. |
| 9–10 | Positioning is a living strategic tool that the product team uses for every major decision. Differentiated value is narrow, specific, and impossible for competitors to claim. Market category choice is deliberate and shapes feature expectations. Pitch is tested across contexts and refined based on feedback. Roadmap investments directly reinforce differentiation. When something doesn't fit the positioning, the team has language to say no. |

## The Five Components of Positioning

Positioning is not a statement — it's a set of five interlocking decisions. Change one and the others must be re-evaluated. These components are not independent: competitive alternatives define what "different" means, unique capabilities ground your differentiation in reality, differentiated value translates capabilities into outcomes, best-fit customers narrow where that value lands hardest, and market category sets the frame through which everything else is interpreted.

### 1. Competitive Alternatives

**Core concept:** Competitive alternatives are what buyers would do if your product didn't exist. This is not a list of named competitors — it's the full set of realistic options a buyer faces, including doing nothing, using spreadsheets, hiring an agency, or building something in-house.

**Why it works:** Competitive alternatives define your frame of reference. If you don't know what you're being compared to, you can't know what "better" means. The alternatives customers actually consider — not the ones you wish they'd consider — determine which capabilities matter and which are irrelevant. Anchoring on real alternatives keeps the rest of the positioning grounded in market reality instead of internal aspiration.

**Key insights:**
- "Do nothing" and "spreadsheet plus duct tape" are almost always alternatives — and often the most dangerous ones, because they're free and familiar
- The alternative set is defined by the buyer's job-to-be-done, not by your competitive intel deck
- Alternatives drift over time as new entrants appear and category lines shift; what you beat last year may not be what you're compared to now
- Different buyer segments evaluate different alternative sets — a SMB buyer rarely considers an enterprise platform, and vice versa

**Product applications:**

| Context | Application | Example |
|---------|-------------|---------|
| Win/loss analysis | Tag every deal with the specific alternative it was compared against | "We lost 60% of mid-market deals to in-house builds, not to our named competitor — the real fight is build-vs-buy" |
| Feature scoping | Only invest in beating the alternatives best-fit buyers actually evaluate | "We don't need parity with the enterprise suite; our buyers are choosing between us and a spreadsheet" |
| Pitch construction | Name the alternatives explicitly in the Setup so differentiation lands | "Teams in your position usually choose between hiring an agency, building internally, or using a point tool — here's why each breaks down" |

**Copy patterns:**
- "If we didn't exist, our best-fit customers would [specific alternative], which means our differentiation has to clearly beat [that alternative], not the competitor we obsess over internally."
- "Our real competitor isn't [named vendor] — it's the spreadsheet plus the manual process. That's what we have to displace."
- "Before we talk about features, let's agree on what you'd do instead — that's the comparison that actually matters."

**Ethical boundary:** Don't strawman the alternatives. Represent what buyers would actually do — including the ways "do nothing" or a competitor might genuinely be the right choice for some segments.

See: [references/five-components-of-positioning.md](references/five-components-of-positioning.md)

### 2. Unique Capabilities

**Core concept:** Unique capabilities are what your product or company can do that alternatives cannot. These are facts, not claims — specific features, architectural decisions, data assets, expertise, or delivery models that are genuinely unique to you.

**Why it works:** Unique capabilities are the raw material for every differentiation claim. If you can't name what's actually unique, you'll default to generic benefits ("faster," "easier," "more flexible") that any competitor could claim. This component is also the direct link to your roadmap — investments should strengthen capabilities that feed differentiation, not chase parity on features competitors already ship.

**Key insights:**
- A unique capability is something an alternative cannot replicate without significant architectural, data, or organizational change — not just something they haven't gotten around to yet
- Both product capabilities (features, architecture) and company capabilities (proprietary data, exclusive partnerships, deep domain expertise) count
- Capabilities decay; what was unique two years ago may be table stakes today
- A long list of "unique" capabilities usually means none of them are — narrow to the few that genuinely separate you

**Product applications:**

| Context | Application | Example |
|---------|-------------|---------|
| Roadmap prioritization | Weight investments that deepen unique capabilities over parity features | "Of these ten requests, only two extend our data-graph advantage — those are Q1; the rest are parity bets we'll only fund if a deal is blocked" |
| Quarterly positioning audit | Re-test each "unique" capability against current competitor releases | "Vendor X shipped real-time sync last month — our 'real-time' claim is now table stakes; we need a new edge" |
| Build-vs-buy decisions | Build what is uniquely yours; buy what is undifferentiated infrastructure | "Auth and billing are not where we differentiate — buy. Our scoring engine is our moat — build." |

**Copy patterns:**
- "We can do [X] because of [specific architectural or data advantage] — alternatives can't replicate this without rebuilding [Y]."
- "Here's what's genuinely unique to us, and here's what's table stakes we just happen to do well — let's not confuse the two on the roadmap."
- "If a competitor could ship this in a sprint, it's not a unique capability — it's a feature."

**Ethical boundary:** Don't claim uniqueness you can't defend in a customer call. Inflated capability claims survive marketing review but collapse in a technical evaluation, destroying trust.

See: [references/five-components-of-positioning.md](references/five-components-of-positioning.md)

### 3. Differentiated Value

**Core concept:** Differentiated value is the business outcomes your unique capabilities create, stated comparatively. Not "we save time" but "we reduce implementation time from six weeks to eight days because we handle the data migration — alternatives hand you documentation and a Slack channel."

**Why it works:** Differentiated value is the bridge between product decisions and market outcomes. It's where capability becomes consequence. Every feature request can be evaluated against it: does this strengthen our differentiated value, or is it a distraction? It's also what your stakeholders, salespeople, and champions need to be able to articulate in one sentence — if they can't, the pitch falls apart in every conversation you're not in.

**Key insights:**
- Every value claim must survive two tests: "So what?" (push to business outcome) and "Compared to what?" (ensure uniqueness)
- Outcomes are stronger than features, and comparative outcomes are stronger than absolute outcomes
- Differentiated value should be narrow — two or three specific claims, not a list of ten
- If a competitor could put the same sentence on their website with a straight face, it's not differentiated value

**Product applications:**

| Context | Application | Example |
|---------|-------------|---------|
| Roadmap filtering | Score features on whether they make differentiated value more true, more defensible, or more visible | "This integration is nice but doesn't reinforce our 'fastest time-to-first-insight' claim — deprioritize" |
| Stakeholder enablement | Test if sales, CS, and execs can restate the differentiated value unprompted | "Three out of five execs described us differently — we need an alignment session before the QBR" |
| Pricing and packaging | Build pricing tiers around the differentiated value, not around feature count | "Our premium tier should monetize the migration speed advantage, not bundle random extras" |

**Copy patterns:**
- "Customers like you get [specific measurable outcome] in [timeframe], compared to [specific outcome from named alternative] — and the reason is [unique capability]."
- "Our differentiated value, in one sentence: [X outcome] for [Y customer], faster/cheaper/more reliably than [named alternative], because [unique capability]."
- "If this feature ships, does our differentiated value statement become more true? If not, why are we building it?"

**Ethical boundary:** Differentiated value claims must be verifiable with customer evidence. Aspirational claims that current customers can't substantiate are a credibility liability, not a marketing asset.

See: [references/differentiated-value-development.md](references/differentiated-value-development.md)

### 4. Best-Fit Customers

**Core concept:** Best-fit customers are the segment that captures maximum value from your differentiation. They're defined by observable characteristics — industry, company size, team structure, growth stage, tech stack, or specific situation — that make your differentiated value disproportionately important to them.

**Why it works:** Best-fit customer definition is the foundation of discovery focus, roadmap targeting, and go-to-market efficiency. Building for everyone means differentiating for no one. When you know exactly who gets the most value from your product, discovery research gets sharper, feature prioritization gets clearer, win rates climb in the chosen segment, and "not for us" becomes a legitimate, strategic response instead of a defensive one.

**Key insights:**
- Best-fit is observable, not psychographic — "ambitious teams" is not a segment; "Series B-to-C SaaS companies with a dedicated RevOps function" is
- Best-fit customers buy fastest, expand most, churn least, and refer most — usage and revenue data will reveal them if you look
- Saying yes to non-best-fit customers in the short term often drags the roadmap toward mediocrity in the long term
- Best-fit shifts as competitive alternatives shift — the segment that loved you when you were the only option may no longer be your sweet spot

**Product applications:**

| Context | Application | Example |
|---------|-------------|---------|
| Discovery research | Recruit interview participants who match best-fit, not whoever responds first | "Our last research round was 70% non-best-fit — no wonder the insights pointed away from our positioning" |
| Roadmap evaluation | Treat requests from outside the best-fit segment as signal, not as requirements | "Three enterprise prospects asked for SSO; none of them are best-fit. We'll note the pattern but not commit roadmap time" |
| Sales qualification | Use best-fit criteria to disqualify fast and protect the team's focus | "If a prospect isn't in our best-fit profile, the rep can pass on them without escalation — we don't chase bad-fit revenue" |

**Copy patterns:**
- "Our best-fit customer is [observable profile]. Everyone else is a bonus, not the plan — and not a roadmap driver."
- "We win deals fast, expand accounts, and get referrals from [specific segment]. That's not a coincidence — that's where our differentiation pays off most."
- "This request comes from outside our best-fit segment. We can listen, but we shouldn't reshape the roadmap for it."

**Ethical boundary:** Be honest with non-best-fit prospects rather than selling them a product that won't deliver value. Closing bad-fit deals creates churn, support burden, and reference risk that costs more than the revenue gained.

See: [references/five-components-of-positioning.md](references/five-components-of-positioning.md)

### 5. Market Category

**Core concept:** The market category is the frame buyers use to understand what you are. It's the mental container that sets expectations for features, pricing, competitors, and buying process. Choosing "project management tool" vs. "work operating system" vs. "team collaboration platform" activates entirely different comparison sets in the buyer's mind.

**Why it works:** Market category choice has direct product implications. Buyers in a category expect certain features as table stakes. Choosing a category means accepting those expectations — or deliberately choosing a different category where your strengths are advantages rather than gaps. The frame determines who you're compared to, how you're evaluated, and how much context you have to set before differentiation can land. This is a product decision, not a marketing decision.

**Key insights:**
- Every category carries table-stakes expectations; entering one means committing to meet them or deliberately reframing
- A category choice that obscures your strengths is a strategic error, even if the category is "bigger"
- Creating a new category is expensive — you trade comparison for education, and education takes time, budget, and a product that genuinely doesn't fit existing frames
- The same product can occupy different categories for different segments; consistency matters more within a segment than across the whole market

**Product applications:**

| Context | Application | Example |
|---------|-------------|---------|
| Roadmap planning | Map table-stakes features for the chosen category and close real gaps | "Buyers in the 'modern data platform' category expect lineage and governance — if we want this frame, we need both on the roadmap" |
| Competitive analysis | Re-evaluate the competitive set whenever you consider a category shift | "If we reframe from 'CRM' to 'revenue platform,' our comparison set changes from Salesforce to a different list — does that help or hurt us?" |
| Launch strategy | Decide whether to fit an existing category, dominate a niche, or create a new one before writing a single piece of launch copy | "We chose 'big fish, small pond' in vertical X — every launch asset reinforces that niche, not the broad category" |

**Copy patterns:**
- "We're positioning in the [specific category] because that's where our differentiation reads as an advantage, not a gap."
- "Table stakes for this category are [X, Y, Z]. We meet them. Our edge is [unique capability], which the category leaders don't have."
- "We could call ourselves a [bigger category], but then we'd be compared to [stronger players] on features we don't lead on. The narrower frame helps us."

**Ethical boundary:** Don't claim a category your product can't credibly deliver against. Buyers who arrive expecting category norms and find a different product feel misled, even if the underlying product is good.

See: [references/market-category-strategies.md](references/market-category-strategies.md)

## The 10-Step Positioning Process

Positioning is not brainstormed — it's derived through a sequential process. The order matters because each step depends on the outputs of the previous steps. Dunford designed this process from hundreds of positioning engagements; shortcuts that skip steps produce positioning that sounds right but falls apart under market pressure.

**Step 1: Assemble a cross-functional positioning team.** Include product, marketing, sales, customer success, and a senior leader who can make binding decisions. Positioning done in a silo gets overridden by the first salesperson who disagrees.

**Step 2: Start with your competitive alternatives.** Don't start with what you are — start with what your customers would do without you. List every realistic alternative, including doing nothing. This grounds the entire exercise in market reality.

**Step 3: Identify your unique capabilities.** For each competitive alternative, ask: what can we do that they can't? Be ruthlessly honest — "we have better UX" is not a unique capability unless you can point to something specific they architecturally cannot replicate.

**Step 4: Map capabilities to differentiated value.** For each unique capability, ask "so what?" until you reach a business outcome, then "compared to what?" until the outcome is genuinely comparative. Discard capabilities that don't produce differentiated value.

**Step 5: Identify your best-fit customers.** Which customer characteristics make your differentiated value disproportionately important? These are the customers who buy fastest, get the most value, churn least, and refer most. Define them by observable characteristics, not psychographics.

**Step 6: Choose your market category.** Based on your competitive alternatives, differentiated value, and best-fit customers, what frame makes your strengths most obvious? This may or may not be the category you started in.

**Step 7: Identify relevant trends (optional).** If a market trend makes your positioning more urgent or credible, name it — but only if it's real, relevant to your best-fit customers, and doesn't substitute for actual differentiation.

**Step 8: Test positioning internally.** Present the positioning to salespeople, customer success, and executives. Watch for confusion, resistance, or inability to restate it. Internal alignment is a prerequisite for market alignment.

**Step 9: Translate positioning into pitch.** Map each positioning component to its pitch equivalent (see the two-phase model below). This is where positioning becomes operational.

**Step 10: Commit and iterate.** Positioning is a living document. Review quarterly. Update when competitive alternatives shift, when you ship capabilities that change your differentiation, or when your best-fit customer profile evolves.

**PM-specific considerations:**
- Steps 1–6 should happen in a single intensive workshop (half-day to full day), not spread across weeks of async review
- The PM's role is facilitator, not sole author — positioning reflects the full team's market knowledge
- Step 5 (best-fit customers) directly feeds your discovery research plan
- Step 6 (market category) directly affects your feature expectations and competitive framing
- Steps 8–10 are ongoing PM responsibilities, not one-time deliverables

See: [references/ten-step-positioning-process.md](references/ten-step-positioning-process.md)

## Market Category Strategies

Your market category isn't just a label — it's a strategic choice that determines which competitors you face, which features buyers expect, and how much context-setting your pitch requires. Dunford identifies three fundamental strategies.

### Head-to-Head

**Compete directly in an existing, well-understood category.** Buyers already know what "CRM" or "analytics" or "project management" means. You accept the comparison set and differentiate within it.

**When to use:**
- Your differentiation is strong enough to win in direct comparison with established players
- The category has well-understood buyer expectations you can meet or exceed
- Buyers are actively shopping in this category and know what they're looking for

**Product implications:** You must meet table-stakes feature expectations for the category. Gaps in expected features count against you more heavily than extra capabilities count for you. Your differentiation must be in areas buyers in this category actually care about.

### Big Fish, Small Pond

**Dominate a niche within an existing category.** You don't claim to be the best CRM — you claim to be the best CRM for real estate teams, or for companies with complex multi-currency pricing.

**When to use:**
- You can't win head-to-head against the category leader across the full market
- A specific segment values your differentiation far more than the broad market does
- The niche is large enough to build a meaningful business in

**Product implications:** Double down on the needs of your chosen niche. Features that serve the niche deepen your moat; features that broaden your appeal dilute it. Your roadmap should make you indispensable to the niche, not adequate for everyone.

### Create a New Category

**Define a new market frame where you set the rules.** Buyers don't have an existing comparison set, so you control the narrative — but you also carry the burden of educating every buyer on what the category is and why it matters.

**When to use:**
- Existing categories force unfavorable comparisons that obscure your real value
- Your product genuinely doesn't fit existing categories without distortion
- You have the resources (time, marketing budget, customer patience) to educate the market

**Product implications:** Category creation requires the product to deliver on the category promise from day one. You can't define a new category and then ship a product that looks like the old category with a new name. Every product decision must reinforce the category narrative.

See: [references/market-category-strategies.md](references/market-category-strategies.md)

## From Positioning to Pitch: The Two-Phase Model

Positioning tells you what to say. The pitch tells you how to say it, in what order, and adapted to whom. Dunford's pitch model has two phases — Setup and Follow-Through — that apply whether you're pitching to a buyer, presenting to executives, updating the board, or aligning cross-functional partners.

### Phase 1: The Setup

The Setup creates the context that makes your product's value land. Without it, your differentiation sounds like marketing copy. With it, it sounds like a logical conclusion.

**1. Market Insight** — Open with a specific, experience-grounded observation about the problem space. This establishes credibility and demonstrates you understand the audience's world.

- For a buyer: "The pattern we see across companies in your segment is…"
- For an exec review: "The market signal we're tracking that has the biggest implications for our roadmap is…"
- For a board update: "The competitive dynamic that changed this quarter is…"

**2. Alternatives** — Walk through the realistic options. In a sales context, these are competitive products. In a stakeholder context, these might be competing strategic directions, build-vs-buy options, or different investment priorities.

- For a buyer: "Companies in your position are typically choosing between…"
- For an exec review: "The approaches we evaluated and why we chose this direction…"
- For a board update: "The strategic alternatives the team considered…"

**3. Perfect World** — Describe what an ideal solution looks like, based on the market insight and the limitations of alternatives. This creates the evaluation criteria before your product enters the conversation.

- For a buyer: "Given these trade-offs, the ideal solution for your situation would…"
- For an exec review: "The outcome we should be optimizing for is…"
- For a board update: "The market opportunity we're positioning to capture requires…"

### Phase 2: The Follow-Through

The Follow-Through delivers your product's story into the context the Setup created.

**4. Introduction** — Position your product (or your proposal) within the landscape you just described. The audience should already have a mental model for where you fit.

**5. Differentiated Value** — The specific outcomes only you deliver, compared to the alternatives discussed. This is the core claim. It must be narrow, specific, and impossible for alternatives to claim verbatim.

**6. Proof** — Evidence matched to the audience's context. For buyers: case studies, demos, data. For executives: metrics, customer evidence, market validation. For boards: strategic evidence, competitive position data, growth indicators.

**7. Objection Handling** — Proactively address the concerns this specific audience will have. Anticipating objections signals confidence and thoroughness.

**8. The Ask** — A specific, clear next step. For buyers: a concrete action with a date. For executives: a decision or resource commitment. For boards: strategic direction approval.

**Why the two-phase model works across contexts:** The Setup/Follow-Through structure works because it mirrors how persuasion actually operates — people need context before they can evaluate a claim. This is true whether you're selling a product, proposing a roadmap direction, or defending a strategic bet.

See: [references/positioning-to-pitch-translation.md](references/positioning-to-pitch-translation.md)

## Differentiated Value: The Bridge Between Product and Market

Differentiated value is the single most important output of the positioning process and the most common point of failure. It connects what your product uniquely does to why that matters in the market — and it's the decision filter for your roadmap.

### The "So What / Compared to What" Test

Every value claim must survive two questions:

**"So what?"** — Push from capability to business outcome. Keep asking until you reach something a stakeholder, executive, or customer would care about.

> "We have real-time data sync" → So what? → "Decisions are based on current data" → So what? → "Your ops team catches inventory issues before they become stockouts" → **Business outcome reached.**

**"Compared to what?"** — Ensure the outcome is genuinely unique to your approach. If a competitor could make the same claim, you haven't finished.

> "Catches inventory issues before stockouts" → Compared to what? → "Compared to the 15-minute polling interval of the two leading alternatives, which means stockout events between polls are invisible until it's too late."

### How Differentiated Value Informs Feature Prioritization

This is where positioning becomes a product management tool, not just a marketing exercise:

- **Features that strengthen differentiated value** deserve priority — they widen the gap between you and alternatives
- **Features that achieve parity** on table-stakes expectations deserve investment only when the gap is blocking deals or causing churn
- **Features requested by customers outside your best-fit segment** should be questioned — they may pull differentiation toward the center
- **Features that any competitor could also build** don't strengthen differentiation — they're parity moves at best

**The roadmap test:** For any proposed feature, ask: "Does this make our differentiated value statement more true, more defensible, or more valuable to our best-fit customers?" If the answer is no, it needs a different justification.

See: [references/differentiated-value-development.md](references/differentiated-value-development.md)

## Proof and Validation

Positioning claims without evidence are just opinions. PMs need to build a portfolio of proof that validates their positioning across different contexts and audiences.

### Types of Proof for PMs

| Proof Type | PM Context | How to Build It |
|------------|-----------|-----------------|
| Customer evidence | Win/loss interviews, usage data, testimonials | Systematic win/loss analysis focused on why customers chose you over specific alternatives |
| Quantified outcomes | Business metrics from deployed customers | Partner with customer success to collect before/after data from best-fit customers |
| Product demonstration | Live or recorded demos of differentiated capabilities | Build demo scenarios that specifically highlight what alternatives can't do — not a feature tour |
| Competitive validation | Third-party comparisons, analyst coverage, review sites | Track where analysts and review sites place you; correct mispositionings proactively |
| Internal alignment | Consistent story across all customer touchpoints | Test whether sales, marketing, and CS can articulate the same differentiated value |

### Building Evidence for Positioning Claims

**For stakeholder pitches (exec reviews, board updates):**
- Lead with metrics: customer adoption, win rates against specific alternatives, retention in best-fit segment
- Use customer quotes that specifically reference your differentiated value, not generic satisfaction
- Show competitive evidence: deals won against named alternatives, analyst positioning, market share in your niche

**For buyer conversations:**
- Match proof to the buyer's profile: industry, size, use case, and the specific outcome they care about
- A single deeply matched case study outweighs ten logo slides
- Live demos structured as proof of differentiation — not feature tours — are the most powerful format

**For cross-functional alignment:**
- Share win/loss data that validates or challenges positioning assumptions
- Use customer interview quotes that surface how customers describe your product versus how you describe it
- Track whether the language customers use matches your positioning language — gaps indicate positioning drift

### Product Demos as Positioning Validation

Demos should prove your positioning is true, not show everything your product does.

**Weak demo structure:** Walk through features in the order they appear in the product navigation.

**Strong demo structure:** Set up the problem (the market insight), show how alternatives handle it (their limitations), then demonstrate how your product handles it differently (your unique capability in action, producing differentiated value the audience can see).

## Common Mistakes

| Mistake | Why It Fails | Fix |
|---------|-------------|-----|
| Treating positioning as a marketing exercise | Positioning that doesn't inform product decisions is just messaging — it drifts from reality as the product evolves | Involve product and engineering in positioning; use it as a roadmap filter |
| Positioning by aspiration rather than reality | Claiming a market position your product can't defend under scrutiny destroys trust with everyone — buyers, analysts, internal teams | Position based on current capabilities; use roadmap to close gaps between current and aspirational positioning |
| Trying to position for everyone | Broad positioning differentiates from no one; every claim becomes generic | Narrow to best-fit customers; accept that excluding some segments makes you stronger in others |
| Skipping competitive alternatives | Without knowing what you're compared to, you can't know what "different" means | Start every positioning exercise with competitive alternatives — it's step one for a reason |
| Confusing features with differentiated value | "We have X feature" is not a value claim; it requires "so what" and "compared to what" | Run every claim through the two-question test before it appears in any pitch |
| Choosing a market category for prestige | Picking a category because it sounds bigger or more impressive, rather than one where your strengths are advantages | Choose the category where your differentiated value is most obvious to buyers |
| Setting and forgetting positioning | Market dynamics shift; competitors ship new capabilities; best-fit customers evolve | Review positioning quarterly; update when competitive alternatives change or new capabilities ship |
| Different teams telling different stories | Sales says one thing, marketing another, product a third — buyers encounter contradictory signals | Use positioning as the single source of truth; audit alignment quarterly |
| Pitching without the Setup | Jumping to your product before establishing context means differentiation lands as marketing copy | Always establish market insight, alternatives, and ideal criteria before introducing your product or proposal |
| Building roadmap without positioning filter | Every feature request seems equally valid when there's no strategic filter | Use differentiated value and best-fit customer definition as explicit prioritization criteria |

## Quick Diagnostic

| Question | If No | Action |
|----------|-------|--------|
| Can you name the top 3 competitive alternatives your best-fit customers actually consider? | You don't know what you're being compared to | Map competitive alternatives from customer interviews and win/loss data, not from your assumptions |
| Can you state your differentiated value in one sentence that names a specific outcome and a comparison point? | Your differentiation is too vague to drive decisions | Run the "so what / compared to what" process until you reach specificity |
| Does your best-fit customer definition use observable characteristics, not psychographics? | You can't reliably identify or target your best customers | Redefine using company size, industry, team structure, growth stage, or specific situation |
| Does your roadmap explicitly reference positioning when prioritizing features? | Positioning and product development are disconnected | Add "positioning impact" as a prioritization criterion; score features against differentiated value |
| Can every team member who talks to customers describe the product the same way? | Different touchpoints send contradictory signals | Run an alignment session; use positioning as the shared narrative |
| Have you reviewed your positioning in the last 90 days? | Competitive landscape and product capabilities have likely shifted | Schedule a quarterly positioning review with cross-functional stakeholders |
| Does your pitch adapt to different audiences (buyers, executives, board, partners)? | You're using a one-size-fits-all story that resonates with no one | Map the two-phase model to each audience context; customize Setup and proof for each |
| Do your product demos prove your differentiation, or just show features? | Demos aren't reinforcing your positioning | Restructure demos around the market insight → alternatives → your unique approach narrative |
| Have you validated your positioning claims with customer evidence? | Positioning is based on internal assumptions, not market reality | Collect win/loss data, customer quotes, and usage metrics that validate or challenge each claim |
| Does your market category choice reflect where your strengths are advantages? | You may be competing on unfavorable terms | Evaluate whether a different category frame would make your differentiation more obvious |

## Reference Files

- [Five Components of Positioning](references/five-components-of-positioning.md) — Deep dive on each component with templates, worked examples, and PM-specific application guidance
- [Ten-Step Positioning Process](references/ten-step-positioning-process.md) — Step-by-step facilitation guide with timing, who to include, and decision-making protocols
- [Market Category Strategies](references/market-category-strategies.md) — When to use each strategy, worked examples, decision framework, and product implications
- [Positioning to Pitch Translation](references/positioning-to-pitch-translation.md) — How the five positioning components map to the eight pitch components, with PM-specific contexts including exec reviews, board updates, and partner conversations
- [Differentiated Value Development](references/differentiated-value-development.md) — Worksheets for the "so what / compared to what" process, connecting differentiation to roadmap decisions

## Further Reading

- [Obviously Awesome by April Dunford](https://www.amazon.com/dp/1999023005?tag=wondelai00-20) — Primary source for the five-component positioning framework and the 10-step positioning process
- [Sales Pitch by April Dunford](https://www.amazon.com/dp/B0C3GN64PT?tag=wondelai00-20) — Primary source for the two-phase pitch model and the positioning-to-pitch translation
- [Good Strategy Bad Strategy by Richard Rumelt](https://www.amazon.com/dp/0307886239?tag=wondelai00-20) — Complementary framework for ensuring your positioning reflects a coherent strategy, not just aspirational messaging
- [Crossing the Chasm by Geoffrey Moore](https://www.amazon.com/dp/0062292986?tag=wondelai00-20) — Essential context on market category dynamics, segment targeting, and the "big fish, small pond" approach to market entry

## About the Author

April Dunford is a positioning consultant and former VP of Marketing who has led go-to-market strategy for over two dozen B2B technology companies. She developed the five-component positioning framework in *Obviously Awesome* from fifteen years of first-hand experience repositioning products at companies ranging from early-stage startups to IBM. *Sales Pitch* extends that positioning work into the conversation layer, providing a structured two-phase model for translating strong positioning into pitches that build confidence and close deals. Her work emphasizes that positioning is not a messaging exercise — it's a strategic decision that determines competitive context, feature expectations, and market perception.
