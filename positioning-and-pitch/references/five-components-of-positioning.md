# Five Components of Positioning

Positioning is not a statement you write — it's five interlocking decisions that define how your product fits into the market. Each component depends on the others, and changing one forces re-evaluation of the rest. This reference provides deep dives, templates, and worked examples for each component, with specific guidance for product managers on how positioning decisions feed product strategy.

---

## Why Five Components, Not One

Many teams reduce positioning to a single statement: "We are X for Y." This compression loses the strategic structure that makes positioning useful. A positioning statement is the output of the five components, not a substitute for them. Teams that skip the components and jump to the statement end up with positioning that sounds good in a slide deck but can't survive a customer conversation, an analyst briefing, or a product prioritization debate.

Each component answers a different question:

| Component | Question It Answers | Why It's Separate |
|-----------|-------------------|-------------------|
| Competitive alternatives | What would buyers do without us? | Defines the comparison frame; everything else is relative to this |
| Unique capabilities | What can we do that alternatives can't? | Grounds differentiation in reality; prevents aspirational claims |
| Differentiated value | What outcomes do those capabilities create? | Connects product to market; makes differentiation matter to buyers |
| Best-fit customers | Who cares most about this value? | Focuses strategy; prevents building for everyone |
| Market category | What frame makes our strengths obvious? | Sets buyer expectations; determines competitive set |

---

## Component 1: Competitive Alternatives

### What This Component Covers

Competitive alternatives are not your competitor list. They're the full set of realistic options a buyer faces when solving the problem your product addresses. This includes:

- **Direct competitors** — products in the same category with the same stated purpose
- **Adjacent solutions** — products from neighboring categories that buyers use as workarounds (e.g., spreadsheets for project management, email for collaboration)
- **In-house/DIY** — building a solution internally, especially common in engineering-led organizations
- **Services** — hiring an agency, consultant, or contractor to solve the problem manually
- **Do nothing** — maintaining the status quo, which is always an option and often the most common "competitor"

### Template: Competitive Alternatives Map

| Alternative | Type | Genuine Strengths | Key Trade-offs | When It's the Right Choice |
|-------------|------|------------------|----------------|---------------------------|
| | Direct / Adjacent / DIY / Service / Status quo | | | |
| | | | | |
| | | | | |
| | | | | |
| Do nothing | Status quo | No cost, no change management, no risk of a bad vendor choice | [Quantify: cost of inaction over 6-12 months] | Only if the problem is genuinely not painful enough to justify any investment |

### Worked Example: B2B Customer Onboarding Platform

| Alternative | Type | Genuine Strengths | Key Trade-offs | When It's the Right Choice |
|-------------|------|------------------|----------------|---------------------------|
| Pendo/WalkMe | Direct | Mature, well-known, broad feature set, strong analytics | Built for feature adoption, not onboarding workflows; requires significant configuration for multi-step onboarding | Teams that need in-app feature adoption guidance more than structured onboarding |
| Internal engineering build | DIY | Full control, no vendor dependency, deeply integrated with your product | Requires ongoing engineering maintenance; onboarding UX is not a core competency for most dev teams; takes 3-6 months to build what a vendor provides day one | Teams with dedicated frontend engineering capacity and highly custom onboarding requirements |
| Customer success team (manual) | Service | High-touch, personalized, catches edge cases a tool would miss | Doesn't scale past ~50 concurrent onboardings; CS team becomes a bottleneck; no self-serve path for smaller customers | Low-volume, high-ACV products where every customer gets white-glove treatment |
| Documentation + email sequences | Adjacent | Low cost, familiar tools, easy to set up | One-size-fits-all; no personalization; no visibility into where customers get stuck; completion rates typically under 30% | Products with simple onboarding that requires more information transfer than workflow guidance |
| Do nothing | Status quo | No cost, no integration effort | Time-to-value stays slow; CS handles repeated questions manually; churn in first 90 days remains elevated | Only if onboarding-related churn is genuinely acceptable |

### PM Application: How Competitive Alternatives Feed Product Decisions

- **Feature comparison scope:** You only need to compare against what your best-fit customers actually consider — not against every product in a Gartner Magic Quadrant
- **"Do nothing" quantification:** Help sales and CS articulate the cost of inaction; this data also supports business cases for internal stakeholder pitches
- **Alternative monitoring:** Set up lightweight tracking (G2 reviews, competitor changelogs, win/loss mentions) to catch when alternatives change their positioning or capabilities
- **Discovery questions:** Derive your discovery questions from the alternatives list — "What approaches have you considered or tried?" maps directly to this component

---

## Component 2: Unique Capabilities

### What This Component Covers

Unique capabilities are the facts — features, architectural decisions, data assets, team expertise, partnerships, or delivery models — that are genuinely unique to your product or company. "Genuinely unique" means a competitor could not claim the same thing without lying or building something they don't currently have.

### The Uniqueness Test

For each capability you list, ask:

1. **Could a direct competitor claim this today?** If yes, it's not unique — it's parity.
2. **Could they build or acquire this in the next 6 months?** If yes, it's a temporary advantage — note the timeline.
3. **Is this a product capability or a company capability?** Both count, but company capabilities (expertise, data, relationships) are often harder for competitors to replicate.
4. **Can you demonstrate this in a product demo or customer reference?** If not, it's aspirational, not current.

### Template: Unique Capabilities Audit

| Capability | Type (Product / Company) | Evidence | Competitor Closest Equivalent | Genuinely Unique? | Durability |
|------------|------------------------|----------|------------------------------|-------------------|------------|
| | | | | Yes / Parity / Temporary | |
| | | | | | |
| | | | | | |

### Worked Example: Developer Experience Analytics Platform

| Capability | Type | Evidence | Competitor Closest Equivalent | Genuinely Unique? | Durability |
|------------|------|----------|------------------------------|-------------------|------------|
| Git-level commit instrumentation (not CI/CD-level) | Product | Measures individual developer workflow patterns, not just pipeline metrics | LinearB measures at PR level; Sleuth at deployment level — neither captures pre-commit workflow | Yes | High — architectural decision, expensive to replicate |
| Benchmark dataset from 2,000+ engineering teams | Company | Customers can compare their metrics against segment-specific baselines | Competitors have smaller datasets; DORA benchmarks are public but not segmented | Yes | Grows with customer base — network effect |
| Non-surveillance design: team-level only, no individual tracking | Product | Architecture physically cannot surface individual developer metrics | Competitors offer individual views with "optional" privacy — customers don't trust the opt-out | Yes — architectural, not a toggle | High — would require rebuilding core data model to change |
| Pre-built dashboards for engineering leadership | Product | 15 templates mapping to common VP Eng reporting needs | Most competitors offer blank-canvas analytics requiring significant setup | Temporary — easy to replicate | Medium — 6-12 months for a competitor to build equivalents |

### PM Application: How Unique Capabilities Feed Roadmap

- **Invest in durable uniqueness:** Prioritize capabilities that are architecturally difficult for competitors to replicate — not features that can be copied in a sprint
- **Audit quarterly:** Competitors ship constantly; what was unique six months ago may be parity today
- **Distinguish between "unique" and "first":** Being first to market with a feature is not the same as having a unique capability — first-mover advantage evaporates when competitors ship the same thing
- **Link to differentiated value:** A unique capability that doesn't produce differentiated value is technically interesting but strategically irrelevant — it should not be a roadmap priority

---

## Component 3: Differentiated Value

### What This Component Covers

Differentiated value is the business outcome your unique capabilities create, stated in comparative terms. It's the answer to "why should I choose you over the alternatives?" expressed as an outcome, not a feature.

### The Structure of a Differentiated Value Statement

```
For [best-fit customer profile],
we're the only [market category] that [specific outcome],
because [unique capability that makes it possible],
which means [business impact] compared to [most common alternative].
```

### Template: Differentiated Value Development

| Field | Your Input |
|-------|-----------|
| Starting capability (from unique capabilities audit) | |
| After "so what?" round 1 | |
| After "so what?" round 2 | |
| After "so what?" round 3 (stop at business outcome) | |
| Primary comparison (which alternative, how specifically?) | |
| Buyer profile where this matters most | |
| Final differentiated value statement | |
| Can a competitor claim this verbatim? (If yes, iterate) | |

### Worked Example: Enterprise Search Platform

| Field | Content |
|-------|---------|
| Starting capability | Federated search across 40+ enterprise data sources without data duplication |
| So what? (1) | Users find information across all company tools from one search bar |
| So what? (2) | Knowledge workers spend less time switching between apps to find what they need |
| So what? (3) | The time from "I need information" to "I have the answer" drops from 20+ minutes of searching across multiple tools to under 30 seconds |
| Primary comparison | Competitors (Elastic workplace search, Coveo) require data indexing and duplication into their system — which means connectors break when source APIs change, and compliance teams flag the data copy as a risk |
| Buyer profile | Companies with 1,000+ employees using 10+ SaaS tools, where information fragmentation is actively slowing decision-making |
| Final statement | "For companies where knowledge workers are searching across 10+ tools to find what they need, we're the only enterprise search platform that queries data in place — no indexing, no data duplication. That means search results are always current, compliance never flags a secondary data store, and you're live in days instead of months. Alternatives that index your data require 6-12 weeks of connector setup and break every time a source API changes." |
| Competitor-proof? | Yes — architectural decision (in-place federation vs. indexing) that competitors cannot claim without rebuilding their core |

### PM Application: Differentiated Value as Roadmap Filter

The differentiated value statement becomes a prioritization tool:

| Feature Request | Does It Strengthen Differentiated Value? | Prioritization Impact |
|----------------|----------------------------------------|----------------------|
| Add 10 more data source connectors | Yes — directly strengthens "queries across 40+ sources" claim | High priority — widens differentiation |
| Build a dashboard builder | No — adjacent feature, not related to search differentiation | Lower priority — parity feature, evaluate based on retention data |
| Improve search relevance ranking | Yes — makes the "under 30 seconds" claim more consistently true | High priority — deepens differentiation |
| Add user management and SSO | Table stakes — doesn't differentiate but blocks enterprise deals | Medium priority — necessary but not differentiating |

---

## Component 4: Best-Fit Customers

### What This Component Covers

Best-fit customers are the segment that gets disproportionate value from your differentiation. They're defined by observable characteristics — not personas, not psychographics, not "innovative companies that value quality."

### The Best-Fit Customer Criteria

Good best-fit customer definitions use characteristics you can observe or discover in the first five minutes of a conversation:

| Observable Criterion | Example | Why It Works |
|---------------------|---------|-------------|
| Company size (employees or revenue) | 200–2,000 employees | Filterable from data; correlates with specific pain points |
| Industry or vertical | Healthcare, fintech, e-commerce | Determines regulatory requirements, buying process, and feature expectations |
| Team structure | Has a dedicated data team but no data engineering function | Identifies the capability gap your product fills |
| Technology stack | Cloud-native infrastructure, uses Snowflake or BigQuery | Indicates integration fit and technical readiness |
| Growth stage or trigger event | Just raised Series B; transitioning from founder-led sales | Correlates with specific urgency and willingness to invest |
| Specific situation | Managing 50+ microservices with no centralized observability | The problem your product solves is acute and urgent |

### Template: Best-Fit Customer Profile

| Dimension | Criteria | Why This Matters for Our Differentiation |
|-----------|---------|----------------------------------------|
| Company size | | |
| Industry / vertical | | |
| Team structure | | |
| Tech stack | | |
| Growth stage / trigger | | |
| Specific situation | | |
| **Summary: Our best-fit customer is…** | | |

### Worked Example: API Monitoring Platform

| Dimension | Criteria | Why This Matters |
|-----------|---------|-----------------|
| Company size | 100–1,000 employees | Large enough to have API complexity; small enough that they don't have a dedicated platform team to build monitoring internally |
| Industry | B2B SaaS, fintech, marketplace platforms | API reliability is directly tied to revenue; downtime = lost transactions |
| Team structure | Has backend engineers but no dedicated SRE or platform team | The gap our product fills — monitoring that doesn't require a platform team to configure and maintain |
| Tech stack | Microservices architecture, 20+ internal APIs | Sufficient complexity that basic uptime monitoring misses the real problems (latency degradation, cascading failures) |
| Growth stage | Post-product-market fit, scaling engineering team from 10 to 50 | Monitoring needs outgrow ad-hoc solutions; this is when the pain becomes acute |
| Specific situation | Experienced a customer-facing API incident in the last 6 months | Recent pain creates urgency and budget |
| **Summary** | B2B SaaS companies with 100-1,000 employees, running 20+ microservices, with backend engineering but no SRE team, who've had a recent API incident | This profile has the pain, the urgency, and the structural gap that makes our no-SRE-required monitoring uniquely valuable |

### PM Application: How Best-Fit Customer Definition Feeds Discovery

- **Recruitment filter:** Interview customers who match the best-fit profile; insights from outside the profile are noise
- **Segment analysis:** Track product metrics (adoption, retention, NPS) segmented by best-fit vs. non-best-fit; the gap validates or challenges your positioning
- **Request triage:** Feature requests from best-fit customers carry more strategic weight than requests from adjacent segments
- **Churn investigation:** If best-fit customers churn, it's a positioning or product crisis; if non-best-fit customers churn, it may be expected

---

## Component 5: Market Category

### What This Component Covers

Market category is the mental frame buyers use to understand what your product is. It's not a label you assign — it's a cognitive container that activates a set of expectations in the buyer's mind: expected features, expected price range, expected competitors, expected buying process.

### Category Choice Has Product Implications

| Category Decision | Product Implication |
|------------------|-------------------|
| Choosing an established category (e.g., "CRM") | You must meet table-stakes feature expectations or buyers reject you before seeing your differentiation |
| Choosing a niche within a category (e.g., "CRM for real estate") | You can skip features the broader category expects but your niche doesn't need; you must go deep on niche-specific needs |
| Creating a new category (e.g., "revenue intelligence platform") | You set the feature expectations, but you also bear the cost of educating every buyer on what the category is |
| Choosing the wrong category | Buyers compare you to products with different strengths; your differentiation doesn't register because the comparison frame is wrong |

### Template: Market Category Evaluation

| Candidate Category | Feature Expectations We'd Need to Meet | Competitive Set It Activates | Does Our Differentiation Stand Out Here? | Education Burden |
|-------------------|--------------------------------------|------------------------------|----------------------------------------|-----------------|
| | | | | |
| | | | | |
| | | | | |

### Worked Example: Collaborative Data Workspace

A product that lets data analysts and business users collaborate on data models and reports. Candidate categories:

| Category | Feature Expectations | Competitive Set | Differentiation Fit | Education Burden |
|----------|---------------------|-----------------|---------------------|-----------------|
| Business intelligence (BI) | Dashboards, visualizations, SQL interface, connectors | Tableau, Looker, Power BI | Poor — our differentiation is in collaboration, not visualization; we'd lose the feature comparison | Low (known category) |
| Data analytics platform | Querying, modeling, governance, scalability | Databricks, dbt, Snowflake | Poor — we'd be compared on data infrastructure, where we're not competitive | Low (known category) |
| Collaborative data workspace | Shared data models, annotation, version control for analysis, business-user access | Few direct competitors | Strong — our collaboration features are the primary value, and the category frame highlights them | High (new-ish category) |

**Decision:** "Collaborative data workspace" makes differentiation most obvious, but requires investment in category education. The PM should budget for more Setup time in every pitch and more educational content in marketing.

### PM Application: Category Choice and Feature Expectations

When you choose a market category, you inherit its table-stakes expectations. Map these explicitly:

| Category | Table-Stakes Features | Do We Have Them? | Gap Priority |
|----------|----------------------|-----------------|-------------|
| [Your chosen category] | | | |
| | Feature 1 | Yes / No / Partial | |
| | Feature 2 | Yes / No / Partial | |
| | Feature 3 | Yes / No / Partial | |

Any "No" on table stakes is a potential deal-breaker that must be addressed in the roadmap or acknowledged honestly in positioning as a deliberate trade-off.

---

## The Interconnection Test

After defining all five components, validate that they're coherent by checking these connections:

| Connection | Test Question | If It Fails |
|------------|--------------|-------------|
| Alternatives → Capabilities | Does each unique capability specifically beat at least one competitive alternative? | You have capabilities without competitive context — they may not matter |
| Capabilities → Value | Does each unique capability translate to a differentiated business outcome? | You have capabilities that are technically interesting but strategically irrelevant |
| Value → Best-fit | Is the differentiated value disproportionately important to the best-fit segment? | Your value is real but your targeting is wrong — or vice versa |
| Best-fit → Category | Do best-fit customers look for solutions in the market category you chose? | Your category doesn't match where your buyers shop — they'll never find you |
| Category → Alternatives | Does the market category activate the right comparison set in buyers' minds? | Your category triggers comparisons where your differentiation doesn't register |

If any connection fails, the positioning needs revision at the point of failure. Don't fix the symptom (e.g., better messaging) — fix the structural disconnect.