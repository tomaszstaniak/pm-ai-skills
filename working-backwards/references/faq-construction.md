# Constructing the FAQ Document

The FAQ is the second half of the PR/FAQ, and in many ways it is the more rigorous half. While the press release tells a compelling customer story, the FAQ pressure-tests that story from every angle. It is where hard questions get asked and honest answers get written down — before the organization commits resources.

At Amazon, the FAQ is split into two sections: the external FAQ (customer-facing questions) and the internal FAQ (business-facing questions). Both are essential. A project that has a strong press release but a weak FAQ is a project that has not been thought through.

## External FAQ: The Customer Perspective

The external FAQ captures questions a real customer would ask after reading the press release. Not questions you wish they would ask. Not questions that let you showcase features. The questions that reveal doubt, confusion, and skepticism.

### How to Generate Authentic Customer Questions

Most teams generate FAQ questions by sitting in a conference room and guessing. This produces questions that are easy to answer because they were written by people who already believe in the product. Instead, use these techniques:

**Technique 1: The Skeptical Friend Test**

Imagine showing the press release to a friend who is not in your industry. What would they ask? They do not care about your technology. They care about:
- Does this actually work?
- How much does it cost?
- What do I have to give up to use this?
- What happens if it breaks?
- How is this different from what I already use?

**Technique 2: Support Ticket Mining**

If you have an existing product, read the last 200 support tickets. The questions customers actually ask are wildly different from the questions product teams expect. Common themes:
- Confusion about pricing and billing
- Fear of data loss or lock-in
- Integration with existing workflows
- What happens when things go wrong
- Privacy and data handling

**Technique 3: The "Yeah, But" Exercise**

Read each sentence of the press release aloud. After each one, have someone respond with "Yeah, but..." and complete the objection. Document every objection.

| Press Release Claim | "Yeah, But" Response | FAQ Question |
|---|---|---|
| "Set up in under an hour" | "Yeah, but what about migration from our current system?" | "How do I migrate my existing data?" |
| "Reduces reporting time by 80%" | "Yeah, but does that include the time to learn the new tool?" | "How long does it take to get proficient?" |
| "Free for teams up to 5" | "Yeah, but what happens when we grow past 5?" | "What does pricing look like as my team scales?" |
| "Works with your existing tools" | "Yeah, but does it work with the specific obscure tool I depend on?" | "Which integrations are available at launch?" |

### Essential External FAQ Categories

Every external FAQ should address these categories, regardless of product type:

**1. Getting Started**
- How do I sign up or purchase?
- What are the system requirements?
- How long does setup take?
- Is there a free trial or free tier?
- Can I import my existing data?

**2. Pricing and Billing**
- How much does it cost?
- What is included in each tier?
- Are there usage limits?
- What happens if I exceed limits?
- Can I cancel at any time?
- Is there a refund policy?

**3. Functionality and Limitations**
- What exactly does the product do?
- What does it not do? (This question is critical and often omitted)
- How accurate/reliable is it?
- What are the known limitations?
- What is on the roadmap?

**4. Trust and Safety**
- How is my data handled?
- Who has access to my data?
- What security certifications do you have?
- What happens if the service goes down?
- Can I export my data if I leave?

**5. Support and Troubleshooting**
- How do I get help?
- What are support hours?
- Is there documentation?
- What is the average response time?

### Writing External FAQ Answers

Rules for writing strong external FAQ answers:

1. **Answer the actual question first.** Do not start with context or caveats. If the question is "How much does it cost?" the first word of the answer should be a price or "Free."

2. **Be specific.** "Affordable pricing" is not an answer. "$29/month for up to 10 users" is an answer.

3. **Acknowledge limitations honestly.** If the product does not do something, say so. "We do not currently support X. We plan to add it in Q3" is far better than dancing around the gap.

4. **Keep answers under 150 words.** If an answer requires more than 150 words, the question is too broad and should be split.

## Internal FAQ: The Business Perspective

The internal FAQ is where the team demonstrates that the business case is sound. These are the questions that leadership, finance, legal, and partner teams will ask. They are harder to answer than external questions because they require analysis, not just description.

### Unit Economics

| Question | What a Weak Answer Looks Like | What a Strong Answer Looks Like |
|---|---|---|
| What is the expected customer acquisition cost? | "We will leverage organic growth and word of mouth." | "Based on comparable products, we estimate $45 CAC through paid search and $12 through content marketing. Blended CAC target is $28, with a 14-month payback period at $29/month ARPU." |
| What are the gross margins? | "We expect healthy margins." | "Infrastructure cost per user is $3.20/month at current scale, dropping to $1.80/month at 10K users. At $29/month pricing, gross margin is 89% at current scale, 94% at target scale." |
| What is the lifetime value? | "Customers will love the product and stay forever." | "Based on industry churn benchmarks of 5% monthly for SMB SaaS, expected LTV is $580. LTV/CAC ratio of 20.7 at blended CAC." |
| When does this break even? | "Within a reasonable timeframe." | "Monthly break-even at 1,200 paying users. Based on growth model, expected 14 months post-launch. Cumulative investment to break-even: $840K." |

### Competitive Landscape

The competitive section must be brutally honest. Pretending competitors do not exist or dismissing them does not help the decision. Leadership needs to understand:

- **Who are the direct competitors?** Products that solve the same problem for the same customer.
- **Who are the indirect competitors?** Products that solve the problem differently, or adjacent products that could expand into your space.
- **What is the status quo competitor?** Often the biggest competitor is "do nothing" or "use a spreadsheet." How entrenched is the current behavior?
- **What is our sustainable advantage?** Not "we have better technology" — that is temporary. What structural advantage do we have? Distribution? Data? Integration? Switching costs?

**Format for competitive analysis in the FAQ:**

| Dimension | Our Product | Competitor A | Competitor B | Status Quo (Spreadsheets) |
|---|---|---|---|---|
| Setup time | 1 hour | 2 weeks | 3 days | None (already using) |
| Monthly cost (50 users) | $145 | $500 | $250 | $0 |
| Key strength | Ease of use | Enterprise features | Integrations | Familiarity |
| Key weakness | Limited enterprise features | Complex setup | Unreliable | Manual, error-prone |
| Target segment | SMB | Enterprise | Mid-market | All |

### Timeline and Dependencies

| Question | Guidance for Answering |
|---|---|
| What is the development timeline? | Break into phases with specific deliverables. Include buffer. Identify the critical path. |
| What are the key dependencies? | List every external dependency: APIs, partnerships, legal approvals, infrastructure. For each, state current status and risk level. |
| What team is needed? | Specific roles and headcount. Distinguish between "need to hire" and "can reassign." Include ramp-up time for new hires. |
| What is the opportunity cost? | What will the team not be working on? Be explicit about trade-offs. |
| What are the key milestones? | Define three to five milestones with dates. Each milestone should be demonstrable, not just "phase 1 complete." |

### Cannibalization and Internal Impact

Questions that teams often avoid but leadership always asks:

- Does this cannibalize an existing product? If so, quantify the impact.
- Does this require changes to existing systems or processes?
- Which other teams need to be involved, and have they agreed?
- Does this create new operational burden (support, maintenance, compliance)?
- What happens to this product if the key people leave?

## How to Answer Hard Questions Honestly Without Killing the Project

The most important skill in FAQ writing is answering hard questions in a way that is honest and constructive. This does not mean sugarcoating. It means structuring the answer so the risk is acknowledged, quantified, and paired with a mitigation plan.

**Framework for hard answers:**

1. **Acknowledge the risk directly.** "Yes, there is a meaningful risk that..."
2. **Quantify the risk.** "Based on [data/comparable], the probability is approximately..."
3. **Describe the mitigation.** "To address this, we plan to..."
4. **Define the tripwire.** "If [specific metric] does not reach [threshold] by [date], we will [pivot/stop/reassess]."

**Example:**

*Q: What if adoption is significantly lower than projected?*

> "This is a real risk. Our projection assumes 8% conversion from free trial to paid, based on industry benchmarks for SMB SaaS. If conversion is 4% or lower after the first 90 days with at least 1,000 trial signups, we will conduct user research to identify the gap. If we cannot identify a clear fix within 30 days, we will recommend sunsetting the product and reallocating the team. Total sunk cost at that decision point would be approximately $320K."

This answer is honest, specific, and actionable. It does not guarantee success, but it shows the team has thought about failure and has a plan for it.

**Answers that kill projects (and should):**

Sometimes the honest answer to a hard question reveals that the project is not viable. That is the FAQ working as designed. It is far better to discover this in a document than after six months of development. If you find yourself unable to write a credible answer to a fundamental question, that is valuable information.

## FAQ Iteration Strategy

The FAQ should go through at least three rounds of iteration:

**Round 1: The Team FAQ**

The product team writes the first draft. This draft will have strong technical answers but weak business and customer answers. That is expected.

**Round 2: The Adversary Review**

Give the PR/FAQ to someone outside the team — ideally someone known for asking hard questions. Their job is to:
- Identify questions that are missing
- Flag answers that are vague or evasive
- Challenge assumptions with "what if" scenarios
- Point out where the FAQ contradicts the press release

**Round 3: The Leadership Preview**

Before the formal review, share the FAQ with one or two senior leaders for informal feedback. They will identify gaps in business logic and strategic alignment that the team may have missed.

**Tracking FAQ iterations:**

| Question | Version 1 Answer | Feedback | Version 2 Answer |
|---|---|---|---|
| "What if the key API partner changes their pricing?" | "We do not expect this to happen." | "This happened to three teams last year. Unacceptable answer." | "API costs are currently 15% of COGS. We have identified two alternative providers. Switching cost is estimated at 3 engineering-weeks. We will maintain integration readiness with one backup provider." |

## Red Flags That Mean the Project Is Not Ready

After completing the FAQ, review it for these warning signs. Any single red flag does not necessarily kill a project, but three or more suggest the concept needs significantly more work before committing resources.

| Red Flag | What It Indicates |
|---|---|
| More than three questions answered with "we need to research this further" | The team does not understand the problem space well enough to commit |
| Unit economics that require best-case assumptions to work | The business model is fragile; any headwind breaks it |
| No credible answer to "why now?" | The problem may be real but the timing may be wrong |
| The competitive section dismisses all competitors | The team has not done genuine competitive analysis |
| Customer quote in the press release sounds like a product manager wrote it | The team is not thinking from the customer's perspective |
| The getting started section requires more than three steps | The product is too complex for the target customer |
| Internal FAQ reveals dependencies on three or more teams that have not been consulted | Execution risk is very high |
| The FAQ avoids the question "what happens if this fails?" | The team has not considered failure scenarios |
| No clear tripwires or kill criteria defined | The project could drift indefinitely without accountability |
| The press release has been rewritten more than five times without converging | The team does not have a clear vision for the product |

## Connecting the FAQ to Decision-Making

The FAQ is not an appendix. It is the analytical foundation for the go/no-go decision. When leadership reads the PR/FAQ, they are evaluating:

1. **Is the customer problem real and significant?** (Press release + external FAQ)
2. **Is the proposed solution compelling?** (Press release + external FAQ)
3. **Is the business case sound?** (Internal FAQ — unit economics, market size)
4. **Can we execute?** (Internal FAQ — timeline, dependencies, team)
5. **What happens if we are wrong?** (Internal FAQ — risks, tripwires, mitigation)

A strong FAQ does not guarantee approval. But a weak FAQ almost always results in a request to "come back when you have better answers." The investment in thorough FAQ construction saves weeks of back-and-forth and builds confidence that the team has done its homework.
