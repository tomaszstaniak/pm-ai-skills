# Positioning to Pitch Translation

Positioning and sales pitching are two different activities that must tell the same story. This reference explains how to take each of the five positioning components from April Dunford's *Obviously Awesome* framework and translate them into specific, actionable pitch elements — with worked examples, anti-patterns, and a practical audit process for teams whose positioning and pitch have drifted apart.

---

## Why Translation Is the Hard Part

Most teams that have done positioning work assume the pitch will follow naturally. It doesn't. Positioning is a strategic document — it describes what you are, for whom, and why. A pitch is a live conversation — it has to build confidence in sequence, across time, in response to a specific person's situation.

The gap between the two shows up in predictable ways: marketing materials accurately reflect the positioning, sales reps describe the product differently in every meeting, and buyers who interact with both come away confused about what they're actually buying. The fix isn't telling salespeople to "read the positioning doc." It's actively translating each positioning component into a pitch element with language, placement, and intent.

---

## The Five Positioning Components and Where They Live in the Pitch

| Positioning Component | What It Describes | Pitch Location | What It Becomes |
|----------------------|------------------|----------------|-----------------|
| Competitive alternatives | What buyers would do if your product didn't exist | Setup — Alternatives | An honest tour of realistic options with genuine trade-offs |
| Unique capabilities | What your product does that alternatives cannot | Follow-Through — Differentiated Value (input) | The specific features or company capabilities that make differentiation real |
| Differentiated value | The outcomes your unique capabilities create | Follow-Through — Differentiated Value (output) | Business results, stated comparatively, that buyers can repeat to stakeholders |
| Best-fit customers | The segment that captures maximum value from your differentiation | Pitch customization layer | Which insight to open with, which proof to use, which objections to prepare for |
| Market category | The frame buyers use to understand what you are | Setup — Market Insight + Introduction | How you describe the problem space and where you place yourself in it |

None of these are one-to-one substitutions. Each translation requires judgment: not everything in your positioning belongs in every conversation, and the way you express positioning in a document differs significantly from how you say it out loud to a buyer who doesn't have the same context your positioning team does.

---

## Component 1: Competitive Alternatives → Setup Alternatives

### The Translation

Your positioning work identifies competitive alternatives not as a competitive battlecard but as an honest answer to "what would the buyer do if we didn't exist?" That's precisely the mindset for the Setup Alternatives section of the pitch.

The Alternatives section isn't a competitive teardown. It's a market map — two to four approaches the buyer could realistically take, each characterized honestly. The buyer who leaves this section should understand the landscape clearly enough to evaluate you fairly, even if they'd never heard of you before.

### Where Teams Get This Wrong

The most common failure: salespeople take the positioning document's competitive alternatives list and convert it into a competitive comparison table where their product wins every row. This signals to buyers that the "comparison" isn't genuine, and it destroys the trust-building purpose of the Alternatives section.

| Anti-Pattern | What It Looks Like | Why It Fails | Fix |
|---|---|---|---|
| Rigged comparison table | 5x5 grid where you check every box and competitors check none | Buyers have seen this format hundreds of times; it reads as fiction | Describe each alternative in its own terms, including where it's genuinely the right choice |
| Competitor as villain | "Company X has had security breaches and doesn't actually support enterprise workflows" | Buyers who have done any research know this is selective; they distrust everything else you say | Name the genuine strength of each alternative before naming where the trade-off shows up |
| Missing the real alternatives | Mapping only direct competitors, ignoring spreadsheets, agencies, or "build it yourself" | Buyers who are actually evaluating a DIY option feel unheard | Ask early: "What approaches are you currently considering?" and map your Alternatives to what you hear |
| Treating "do nothing" as not an alternative | Jumping from alternatives directly to your product | The status quo is your most common competitor; ignoring it lets buyer inertia win | Name "do nothing" explicitly; characterize it honestly (real short-term benefits, real long-term costs) |

### Worked Example: B2B SaaS Data Pipeline Tool

**In positioning document:** Competitive alternatives are (1) custom-built ETL with internal engineering, (2) legacy on-premise tools like Informatica, (3) modern cloud-native competitors like Fivetran and Airbyte, and (4) doing nothing / continuing to manage data movement with scripts.

**In pitch conversation:**
> "Companies in your situation are typically looking at one of four paths. The first is having your own engineering team build and maintain pipelines — this gives you maximum control and you're not dependent on a vendor, but in practice we see the maintenance burden accumulate faster than teams expect, especially as data sources change. The second is older on-premise platforms — they're mature, your procurement team knows how to buy them, but the implementation timeline and the ongoing infrastructure management usually means you're not moving fast. Third are newer cloud-native tools like Fivetran or Airbyte — they're strong for straightforward connectors and getting up quickly; where they run into friction is when your data models are complex or your compliance requirements mean you need to control where data moves. And the fourth option, which is worth naming, is just continuing with what you have — scripts and manual processes that your team knows, even if they're fragile. That's a real choice and it has real costs in analyst time and data reliability, but it's not zero. Does that map to what you're actually weighing?"

This characterizes Fivetran and Airbyte honestly. It doesn't pretend they don't exist or that they're bad products. It locates the trade-off precisely — which is exactly what the buyer needs.

---

## Component 2: Unique Capabilities → Differentiated Value (Input)

### The Translation

Unique capabilities are what you can do that alternatives cannot. In positioning, these are typically product features or company characteristics: a specific algorithm, a proprietary data set, a deployment model, a services capability, or a technology architecture choice.

In the pitch, these are the *input* to differentiated value — not the thing you say to buyers, but the foundation that makes your differentiated value claims true. The mistake is leading with capabilities (feature claims) instead of translating them into outcomes (value claims).

### The Two-Question Test

Run every capability through these two questions before it appears in a pitch:

1. **"So what?"** — Push from the capability to the business outcome it creates. Keep pushing until you reach something a CFO or VP would care about.
2. **"Compared to what?"** — Confirm the outcome is genuinely distinctive. If the answer is "compared to doing it the old way," that's usually not differentiated enough. If the answer is "compared to how Alternative X handles this specific scenario," you're closer.

| Capability | After "So What?" | After "Compared to What?" | Pitch-Ready? |
|---|---|---|---|
| "Real-time data sync" | "Decisions are made on current data, not yesterday's export" | "Competitors sync on 15-minute intervals; for live inventory management that means your picks are based on stale counts" | Yes — specific and comparative |
| "ISO 27001 certified" | "You can pass security reviews faster" | "You can pass reviews without providing additional documentation — most alternatives require you to complete a vendor security questionnaire during every procurement cycle" | Depends — only differentiating if your segment actually experiences this friction |
| "AI-powered" | "Things happen automatically instead of manually" | This is not yet comparative — every competitor also claims AI | No — keep asking "so what?" until you reach a specific automated outcome; keep asking "compared to what?" until you reach a specific alternative |
| "Dedicated onboarding team" | "You reach your first workflow in 8 days instead of 6 weeks" | "Self-serve onboarding from our two main competitors averages 6 weeks to first live workflow, because the customer handles data migration; our team handles it, so your team doesn't need to be involved" | Yes — specific outcome, specific comparison |

### Worked Example: Internal Tools Platform for Engineering Teams

**Unique capability in positioning:** Visual UI builder that generates production-grade code, eliminating the need for a separate front-end engineer on internal tool projects.

**After "so what?":** Engineering teams ship internal tools 4x faster.

**After "compared to what?":** Competitors like Retool also have visual builders, but they generate proprietary configurations that only work inside their platform — any customization beyond their components requires writing React. Our builder generates standard React that your engineers own.

**Pitch language:** "What we do differently is that the code our builder generates is just React — your engineers can open it in VS Code and modify it like anything else in your codebase. Retool's visual builder is faster to start, but you're locked into their component library; anything outside that requires custom JS inside their environment. The distinction shows up when requirements change six months after launch and whoever built the original tool has moved teams."

---

## Component 3: Differentiated Value → Follow-Through Statement

### The Translation

Differentiated value is the output of the translation process — the business outcome your unique capabilities create, stated in terms buyers can repeat internally. This is what your champion says to the CFO. It needs to be short enough to remember, specific enough to be credible, and comparative enough to explain why you, not a competitor.

### Differentiated Value Statement Template

```
For [best-fit customer type], we're the only [market category] that [unique outcome],
because [unique capability that makes it possible], which means [business impact]
compared to [most common alternative].
```

**Filled example (DevSecOps platform):**
> "For engineering teams shipping more than 20 services, we're the only security platform that surfaces exploitable vulnerabilities in production without requiring a dedicated AppSec team, because we integrate directly into your CI/CD pipeline and apply remediation suggestions in the same PR review where code is written — which means you reduce your mean time to remediate from weeks to hours, compared to bolt-on scanners that generate reports someone has to triage separately."

This is longer than a tagline but shorter than a paragraph. It's the core claim that the Follow-Through builds evidence around.

### Common Differentiated Value Anti-Patterns

| Anti-Pattern | Example | Why It Fails | Fix |
|---|---|---|---|
| Feature masquerading as value | "We have 200+ integrations" | Doesn't state an outcome; buyer has to infer why that matters | "You can connect to your existing stack without engineering work, because we have pre-built connectors for the 30 tools your segment uses most" |
| Generic superlative | "The most intuitive interface in the category" | Every product in the category claims this; it's un-verifiable and un-memorable | Name a specific usability outcome: "Non-technical users can build their own reports without analyst support" |
| Outcome without comparison | "Reduces manual data entry by 60%" | Sounds good but doesn't distinguish you from alternatives who could claim similar numbers | "Reduces manual data entry by 60% compared to our two main competitors, because our matching algorithm handles the edge cases that require human review in rule-based systems" |
| Comparison without mechanism | "Faster than Competitor X" | Buyers don't know whether to trust the claim; sounds like a marketing assertion | Add the capability that makes it true: "Faster than Competitor X at initial implementation, because we handle data migration; you don't need to" |

---

## Component 4: Best-Fit Customers → Pitch Customization Layer

### The Translation

Best-fit customers in positioning define who gets maximum value from your differentiation — typically by industry, company size, growth stage, team structure, or specific situation. In the pitch, this becomes the customization layer: the decisions you make before every conversation about which insight to open with, which proof to lead with, and which objections to prepare for.

This is not a persona slide. It's an active filter you apply to every pitch element.

### Customization Decision Framework

Before each meeting, answer:

| Question | How Best-Fit Customer Definition Answers It |
|---|---|
| Which market insight will land? | Insights that describe patterns specific to this buyer's industry, size, or current growth stage |
| Which case study should I lead with? | The one that most closely matches this buyer's profile, use case, and the specific outcome they care about |
| Which differentiated value claim matters most? | The one that connects to the pain they've confirmed — not every differentiation point is relevant to every buyer |
| Which objections should I prepare for? | Objections common to buyers at this stage of growth or in this industry vertical |
| How much Setup does this buyer need? | Buyers from your core segment need less market education; buyers from adjacent segments need more |

### Worked Example: Consumer App Analytics Platform

**Best-fit customers (from positioning):** Mobile consumer apps with >100K MAU that have an in-house data team but no dedicated mobile analytics function — they're using general-purpose analytics tools (Amplitude, Mixpanel) that weren't built for mobile event schemas.

**Before a meeting with a gaming company (good fit):** Lead with insight about how mobile gaming event schemas are categorically different from web app events. Lead proof with a gaming company case study. Prepare for the objection "we already have Mixpanel" with a specific, honest comparison.

**Before a meeting with a B2B SaaS company (adjacent, weaker fit):** The market insight about mobile event schemas is partially relevant — they may have a mobile app — but the core differentiation matters less if mobile is not their primary acquisition channel. Surface this early rather than pitching hard at a buyer who's outside your best-fit profile. The best outcome might be a referral or a "not yet" rather than a confused sale.

### The Qualification Question Your Positioning Should Generate

If you've done positioning work properly, you can derive a 2-3 question qualification check directly from your best-fit customer definition. These belong at the top of discovery, not at the end.

**Example (data pipeline tool):**
1. "How is your current data team structured — do you have dedicated data engineers, or is it more analysts handling their own pipelines?"
2. "What does your current data stack look like — are you working with cloud-native infrastructure, or is some of it still on-premise?"
3. "What's the ratio of data requests coming from the business versus what your team can realistically ship?"

The answers tell you immediately whether this buyer fits the profile for which your differentiation is actually meaningful.

**Copy pattern:** "The companies that get the most value from us are specifically those who [best-fit criteria] — which is why I was interested to talk with you, because you match that profile…"

---

## Component 5: Market Category → Setup Framing

### The Translation

Your market category choice is the frame through which buyers interpret everything else you say. It determines what reference points they use, what alternatives they consider, and how much context they already have.

In the pitch, market category choice shows up in two places:
1. **The Market Insight** — how you describe the problem space and what's happening in it
2. **The Introduction** — how you name what you are when you first mention your product

### Category Type Affects Setup Depth

| Category Type | What It Means | Setup Required |
|---|---|---|
| Existing, well-understood category | Buyer already has a mental model: "CRM," "analytics," "payroll" | Less Setup — buyer has context; focus on why this moment and why your approach |
| Existing category, repositioned | You're claiming a new way of competing within a known frame | Moderate Setup — acknowledge the category, then introduce the new lens |
| New or emerging category | Buyer doesn't have a pre-existing frame | Substantial Setup — you must establish what the problem space is before you can explain where you sit in it |
| Adjacent to existing category | You solve a problem buyers often solve with something from a neighboring category | Careful Setup — establish why the adjacent tool isn't purpose-built, before introducing the category |

### Worked Example: New Category (Buyer Enablement Platform)

A company that helps sales teams give buyers self-service access to deal materials — contracts, technical docs, demo recordings — might call this a "buyer enablement platform," a category most buyers haven't heard of.

**Wrong opening (no category framing):**
> "We help sales teams close deals faster by giving buyers a portal for deal materials."

This lands as "a file-sharing tool for sales." The buyer doesn't know what to compare it to or why it matters.

**Right opening (category framing in the Setup):**
> "One pattern we see consistently in enterprise B2B deals is that after the demo, the buying process moves to people who weren't in the room — legal, IT, the CFO — and those people are working from memory, from notes, or from materials forwarded through email chains. The seller has no visibility into what they're looking at, when, or what questions they have. The deal lives or dies in a process the seller can't participate in. The category that's emerging to address this is buyer enablement — giving the seller a presence inside the buying process, not just at the demo."

Now the Introduction lands: "That's what we do — we're a buyer enablement platform."

### The Introduction Placement Rule

A common mistake is introducing the product before the Setup is complete. The Introduction should come only after the market insight is established and at least some of the alternatives context is set. The buyer needs to understand what they're being introduced *into*.

**Wrong:**
> "Let me tell you about Acme — we're a buyer enablement platform. Before I show you the product, let me share some context about the market…"

**Right:**
> "[Full Setup] … That's the gap we built to address. Acme is a buyer enablement platform — a dedicated space where the deal lives during the buying process, accessible to the full buying team, with full visibility for the seller into who's engaging with what."

**Copy pattern:** "We sit in the [category] space, which means you're probably also looking at [alternatives]. Let me share how we think about where they each fit…"

**Ethical boundary:** Do not use positioning to artificially inflate your market category to seem larger or more established than you are. Buyers who discover the category inflation — through analyst research or competitor conversations — lose confidence in everything else you've told them.

---

## Positioning-to-Pitch Alignment Audit

Run this audit quarterly, or any time you notice inconsistency between what marketing says and what sales says.

| Audit Question | Green | Yellow | Red |
|---|---|---|---|
| Can every sales rep state your best-fit customer profile in one sentence? | All reps can, consistently | Most can, minor variations | Significant variation or confusion |
| Does your pitch Alternatives section match the alternatives in your positioning document? | Exact match | Partial — some alternatives missing | No connection |
| Does your market category appear in your pitch Introduction in the same terms as your positioning? | Exact match | Paraphrased but consistent | Contradictory or absent |
| Is every differentiated value claim in the pitch traceable to a unique capability in your positioning? | All claims traceable | Most traceable, some are general | Claims that can't be grounded in real capabilities |
| Are your proof assets (case studies, data) organized by your best-fit customer segments? | Yes, actively maintained | Some segmentation but incomplete | One-size-fits-all proof library |
| Do SDRs, AEs, and SEs all describe the product in the same category terms? | Consistent across all roles | Mostly consistent, some outliers | Each role has its own framing |

If any row is Red, treat it as a positioning or pitch problem that will cost you deals until it's resolved. Yellow rows are improvement items for the next storyboard session. Green rows should still be reviewed quarterly — category dynamics shift and positioning that was accurate six months ago may need updating.

---

## When Positioning Needs to Be Fixed First

Some pitch problems can't be solved at the pitch layer. If you're encountering any of these signals, the underlying positioning needs work before the pitch can be improved:

- Salespeople can't agree on who the ideal customer is
- The pitch describes a market category that analysts, buyers, or competitors define differently than you do
- Your differentiated value claims are ones competitors could make without lying
- The alternatives discussion consistently surfaces a competitor whose positioning is clearer and easier for buyers to understand
- Marketing materials and sales materials describe the product as solving different problems

In these cases, running a pitch storyboard session will surface the disagreements but won't resolve them. The resolution happens in a positioning exercise — ideally cross-functional, with sales, marketing, product, and customer success — before pitch work resumes.

---

The translation from positioning to pitch is not a one-time project. As your product evolves, your best-fit customer shifts, and the competitive landscape moves, both positioning and pitch need to be updated together. Teams that maintain this alignment treat it as a continuous practice — not a launch deliverable — and their sales conversations stay coherent across every touchpoint a buyer encounters.