# PM AI Skills

Agent skills for Claude Code and agentskills.io-compatible agents. Each skill distills a book from the [product management reading list at tomaszstaniak.com/books](https://tomaszstaniak.com/books) — a curated library of essential reading for product people — into a practical framework you can apply directly in your AI workflows.

## Installation

### Via skills.sh

Install via [skills.sh](https://skills.sh):

```bash
# Install all skills
npx skills add tomaszstaniak/pm-ai-skills

# Or install individual skills
npx skills add tomaszstaniak/pm-ai-skills/continuous-discovery-habits
npx skills add tomaszstaniak/pm-ai-skills/escaping-build-trap
npx skills add tomaszstaniak/pm-ai-skills/first-90-days
npx skills add tomaszstaniak/pm-ai-skills/good-strategy
npx skills add tomaszstaniak/pm-ai-skills/working-backwards
```

## Available Skills

| Skill | Description | Based On |
|-------|-------------|----------|
| [continuous-discovery-habits](#continuous-discovery-habits) | Weekly customer touchpoints using Opportunity Solution Trees and assumption testing | [Teresa Torres](https://x.com/ttorres)' *"Continuous Discovery Habits"* |
| [escaping-build-trap](#escaping-build-trap) | Shift from output-driven feature factories to outcome-driven product teams | [Melissa Perri](https://x.com/lissijean)'s *"Escaping the Build Trap"* |
| [first-90-days](#first-90-days) | Leadership transition framework: STARS diagnosis, early wins, and the 5 key conversations | [Michael D. Watkins](https://x.com/MichaelDWatkins)' *"The First 90 Days"* |
| [good-strategy](#good-strategy) | Evaluate and design real strategy using the kernel: diagnosis, guiding policy, coherent actions | [Richard Rumelt](https://x.com/RichardRumelt)'s *"Good Strategy Bad Strategy"* |
| [working-backwards](#working-backwards) | Amazon's PR/FAQ method for defining customer experience before writing a line of code | Colin Bryar & Bill Carr's *"Working Backwards"* |

---

## Skill Details

### continuous-discovery-habits

Build a weekly cadence of customer touchpoints using Opportunity Solution Trees, assumption mapping, and interview snapshots. Good product teams don't debate opinions — they test assumptions.

**About the author:** [Teresa Torres](https://x.com/ttorres) is an internationally acclaimed author, speaker, and coach who helps product teams adopt continuous discovery practices. Her Opportunity Solution Tree (OST) framework has become a cornerstone of modern product discovery, giving teams a structured way to explore the problem space before committing to solutions. *"Continuous Discovery Habits"* is the definitive guide to making discovery a regular team habit, not a one-time phase. → [Book notes](https://tomaszstaniak.com/books/discovery-and-product-development/continuous-discovery-habits)

**Use when you need to:**
- Build an Opportunity Solution Tree from a desired outcome
- Identify and prioritize customer opportunities from interview data
- Design assumption tests before committing to a solution
- Structure customer interview snapshots for team alignment
- Move from output-driven to outcome-driven product development
- Map current-state customer journeys
- Build a repeatable weekly discovery habit

**Example prompts:**
- *"Help me build an Opportunity Solution Tree for our retention OKR. Use continuous-discovery-habits skill."*
- *"I did 5 customer interviews this week. Help me create an interview snapshot. Use continuous-discovery-habits skill."*
- *"Map the riskiest assumptions for this feature before we build it. Use continuous-discovery-habits skill."*
- *"How do I set up a weekly discovery habit with a small team? Use continuous-discovery-habits skill."*

---

### escaping-build-trap

Diagnostic and corrective framework for product teams stuck in the build trap — the cycle of shipping features without measuring outcomes. Covers PM archetypes, outcome roadmaps, and strategy deployment from vision to team-level decisions.

**About the author:** [Melissa Perri](https://x.com/lissijean) is a product consultant, speaker, and CEO of Produx Labs. She has worked with companies ranging from early-stage startups to Fortune 500 enterprises to help them build product-led organizations. *"Escaping the Build Trap"* diagnoses why most companies become feature factories and provides a path back to building products that actually work for the business.

**Use when you need to:**
- Diagnose whether a team is stuck in the build trap
- Shift from output-driven roadmaps to outcome-based product strategy
- Evaluate PM archetypes and identify gaps in team maturity
- Design a strategy that connects company vision to team-level decisions
- Run a pre-mortem on a product roadmap to detect build-trap patterns

**Example prompts:**
- *"Are we a feature factory? Diagnose our product team using the build trap signals. Use escaping-build-trap skill."*
- *"What PM archetype is this person? Waiter, Former Project Manager, Mini-CEO, or Strategic PM? Use escaping-build-trap skill."*
- *"Convert our feature roadmap into an outcome roadmap. Use escaping-build-trap skill."*
- *"Run a pre-mortem on this roadmap — what build-trap patterns are hiding in it? Use escaping-build-trap skill."*

---

### first-90-days

Structured framework for accelerating leadership transitions. Covers STARS situation diagnosis, the five critical conversations, early win identification, and phase-by-phase 30-60-90 day planning.

**About the author:** [Michael D. Watkins](https://x.com/MichaelDWatkins) is a professor at IMD Business School and co-founder of Genesis Advisers, a leadership development firm specializing in transition acceleration. *"The First 90 Days"* has been translated into over 25 languages and is widely regarded as the essential playbook for anyone starting a new leadership role. It draws on research from hundreds of executive transitions to identify the patterns that determine success or failure.

**Use when you need to:**
- Plan onboarding for a new leadership or management role
- Build a structured 30-60-90 day plan
- Diagnose the business situation you're entering using the STARS model
- Prepare for critical early conversations with your boss, peers, and team
- Identify common transition traps before you fall into them
- Find early wins that build credibility without overreaching

**Example prompts:**
- *"I'm starting a new Head of Product role next week. Build me a 90-day plan. Use first-90-days skill."*
- *"Diagnose my situation using the STARS model. Here's what I know so far. Use first-90-days skill."*
- *"Help me prepare for my first conversation with my new manager. Use first-90-days skill."*
- *"What early wins should I target in my first 30 days as a new engineering manager? Use first-90-days skill."*

---

### good-strategy

Framework for evaluating, designing, and stress-testing strategies using Rumelt's kernel (diagnosis, guiding policy, coherent actions) and Porter's principle of strategic trade-offs. Includes a built-in pre-mortem to detect bad strategy before committing to it.

**About the source:** [Richard Rumelt](https://x.com/RichardRumelt) is a professor at UCLA Anderson School of Management and one of the world's leading strategy researchers. *"Good Strategy Bad Strategy"* cuts through the noise of vague mission statements and goal lists to define what strategy actually is — a coherent response to a real challenge. The skill also incorporates Michael Porter's foundational insight from *"What Is Strategy?"*: that strategy is fundamentally about choosing what not to do. → [Book notes](https://tomaszstaniak.com/books/strategy-and-leadership/good-strategy-bad-strategy)

**Use when you need to:**
- Evaluate whether a strategy is genuine or disguised fluff
- Diagnose the core challenge before proposing solutions
- Build a coherent strategy kernel from scratch
- Stress-test a strategic plan using pre-mortem analysis
- Distinguish real strategy from goals, ambitions, or wish lists
- Identify Porter's activity-fit and competitive trade-offs

**Example prompts:**
- *"Is this a real strategy or bad strategy? Evaluate it against Rumelt's kernel. Use good-strategy skill."*
- *"Help me write the diagnosis for our product strategy. Use good-strategy skill."*
- *"Run a pre-mortem on this strategic plan — what could make it fail? Use good-strategy skill."*
- *"Our strategy says 'be the best platform for X.' Is that a strategy or a goal? Use good-strategy skill."*

---

### working-backwards

Amazon's product development method: start from the customer experience and work backwards to the technology. The centerpiece is the PR/FAQ document — a fictional press release and FAQ written before a single line of code is written.

**About the source:** Colin Bryar (former Chief of Staff to Jeff Bezos) and Bill Carr (former VP of Music and Video at Amazon) spent a combined 27 years at Amazon. *"Working Backwards"* reveals the internal practices that made Amazon one of the most innovative product companies in the world. The PR/FAQ process is the most transferable of these practices — a discipline that forces clarity of thinking before any resources are committed. → [Book notes](https://tomaszstaniak.com/books/organizational-effectiveness/working-backwards)

**Use when you need to:**
- Write a PR/FAQ document for a new product or feature
- Validate an idea by defining the customer experience first
- Stress-test a proposal with a structured pre-mortem
- Align stakeholders around a product vision before building
- Decide whether an idea is worth pursuing before writing code

**Example prompts:**
- *"Write a PR/FAQ for this product idea. Use working-backwards skill."*
- *"Review this PR/FAQ — does the press release make you want the product? Use working-backwards skill."*
- *"Run a pre-mortem on this PR/FAQ. What could make this product fail? Use working-backwards skill."*
- *"Help me write the FAQ section — what are the hardest questions this proposal needs to answer? Use working-backwards skill."*

---

## License

This repository is licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).

**You are free to:**
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material for any purpose, even commercially

**Under the following terms:**
- **Attribution** — you must give appropriate credit to [Tomasz Staniak](https://tomaszstaniak.com), provide a link to the license, and indicate if changes were made
- **ShareAlike** — if you remix, transform, or build upon the material, you must distribute your contributions under the same CC BY-SA 4.0 license

---

## Copyright & Disclaimer

The methodologies and frameworks referenced in these skills are the intellectual property of their respective authors and publishers. All copyrights belong to:

- **Continuous Discovery Habits**: Teresa Torres
- **Escaping the Build Trap**: Melissa Perri
- **The First 90 Days**: Michael D. Watkins
- **Good Strategy Bad Strategy**: Richard Rumelt
- **What Is Strategy?**: Michael E. Porter
- **Working Backwards**: Colin Bryar, Bill Carr

These skills were created without directly copying or reproducing content from the original books or materials. They are based on:
- Publicly available information about the methodologies
- General knowledge embedded in large language models
- Common industry practices and terminology

We encourage you to purchase and read the original books for the complete, authoritative treatment of each methodology. The skills in this repository are intended as practical aids, not replacements for the source materials.
