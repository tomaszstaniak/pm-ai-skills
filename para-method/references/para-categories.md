# PARA Categories Deep Dive

The four PARA categories — Projects, Areas, Resources, Archives — are not folders. They are answers to the question "How actionable is this information right now?" This reference provides detailed guidance on categorization decisions, common mistakes per category, examples across different PM roles, and how PARA categories map to the artifacts product teams produce.

---

## The Actionability Hierarchy

PARA's power comes from sorting information by its proximity to current action. The hierarchy creates a natural information flow:

| Category | Actionability Level | Time Horizon | Defining Question |
|----------|-------------------|--------------|-------------------|
| **Projects** | Highest — active right now | Days to months | "What am I trying to finish?" |
| **Areas** | High — ongoing maintenance | Indefinite | "What am I responsible for maintaining?" |
| **Resources** | Medium — potential future use | Variable | "What am I genuinely interested in?" |
| **Archives** | Low — inactive but retrievable | Historical | "What's completed or no longer relevant?" |

Information flows downward over time. A Resource topic becomes a Project when you decide to act on it. A Project becomes an Archive when it completes. An Area spawns Projects and eventually some of its material gets archived when your responsibilities change.

---

## Projects: Detailed Guide

### The Two Tests for a Valid Project

1. **Does it have a specific goal?** "Improve onboarding" is not a project — it has no finish line. "Reduce onboarding drop-off at step 3 by 20%" is a project.
2. **Does it have a deadline?** Even self-imposed deadlines count, but a project without any time boundary is an area in disguise.

### Project Folder Structure

A project folder should contain everything needed to do the work and everything produced by the work:

```
Project: Q2 Pricing Restructure
├── 00-Project-Brief.md (goal, deadline, success criteria)
├── 01-Research/
│   ├── Customer-interview-summaries.md
│   ├── Competitor-pricing-analysis.md
│   └── Industry-benchmarks.md
├── 02-Analysis/
│   ├── Pricing-model-comparison.md
│   └── Revenue-impact-scenarios.md
├── 03-Deliverables/
│   ├── Pricing-recommendation-memo.md
│   └── Board-presentation-slides.md
└── 04-Archive/
    └── Outtakes-and-drafts/
```

### Project List Management for PMs

| Role | Typical Project Count | Warning Sign | Action |
|------|----------------------|-------------|--------|
| IC PM | 5-8 active projects | More than 10 | Audit: which can be paused, delegated, or scoped down? |
| Senior PM | 7-10 active projects | More than 12 | Split: are some of these actually areas, not projects? |
| Group PM / Director | 8-12 active projects | More than 15 | Delegate: which projects should belong to your reports? |
| VP Product | 5-7 strategic projects | More than 10 | Elevate: are you holding projects that should be delegated? |

**Key insight:** Your active project list reveals your actual priorities, regardless of what you claim them to be. If "improve activation rate" is your stated top priority but it doesn't appear as a project, it's not actually a priority — it's a wish.

### Product Applications

| Context | Application | Example |
|---------|-------------|---------|
| Quarterly planning | Audit project list against stated strategic priorities | If 60% of your projects serve one initiative and 10% serve your "top priority," reallocate |
| 1:1s with leadership | Share active project list as a transparency tool | "Here are my 7 active projects. I can add this request, but which one should I drop?" |
| Capacity management | Use project count as a workload signal | More than 10-12 active projects is a sign of overcommitment |
| Handoffs | A project folder contains everything needed to hand off work | New PM can pick up context without a weeks-long knowledge transfer |

### Copy Patterns

- "Project: [verb] [outcome] by [date]" — e.g., "Project: Ship onboarding redesign by April 1."
- "Here are my N active projects — which should I drop to take this on?"
- "Let me check the project folder before we rebuild context from scratch."

**Ethical boundary:** Never use project categorization to hide work from stakeholders. The project list should be an honest reflection of where time goes, not a curated portfolio.

---

## Areas: Detailed Guide

### The Standard Test

Every area must have an associated standard — a minimum acceptable level of quality or performance. If you can't articulate the standard, the area is either poorly defined or is actually a resource (an interest, not a responsibility).

| Area | Standard | How You Know It's Slipping |
|------|----------|---------------------------|
| Product quality | Fewer than 5 critical bugs per release | Bug count rising; customer complaints increasing |
| Team health | Quarterly engagement above 80%; no unplanned attrition | Silent 1:1s; missed deadlines; surprise departures |
| Stakeholder relationships | No surprises in leadership reviews; alignment on priorities | Executives ask questions you should have preemptively answered |
| Customer satisfaction | NPS above 45 in target segment | NPS trending down; qualitative feedback shifting negative |
| Technical debt | Debt-to-feature ratio below 30% of sprint capacity | Engineers start flagging velocity problems; incidents increase |
| Professional development | One new framework or skill per quarter | You're applying the same approaches you used two years ago |

### Areas vs. Projects: The Litmus Test

Ask: "If I did this perfectly for six months and then stopped, would it be done?"

- **Yes** → It's a project. It has a finish line.
- **No** → It's an area. It requires ongoing maintenance.

### PM-Specific Areas

These areas are common across PM roles, though the specific standards vary by level and company:

- Product strategy and vision
- Customer research and insight
- Cross-functional relationships
- Team culture and operations
- Market and competitive awareness
- Professional development and growth
- Stakeholder communication
- Data and analytics practice

### Product Applications

| Context | Application | Example |
|---------|-------------|---------|
| Role transitions | Areas change when responsibilities change | Promoted to group PM: "individual product quality" becomes "portfolio quality" |
| Performance reviews | Areas map to the standards you're measured against | "These are my 8 areas of responsibility. Here's how I'm performing against each standard." |
| Delegation | Clearly define which Areas transfer when delegating | "I'm handing the 'vendor relationships' area to you. Here's the folder with all context." |
| Onboarding | New PMs inherit Area folders with accumulated context | Instead of tribal knowledge, the new PM gets a structured repository of standards and reference material |

### Copy Patterns

- "Area: [responsibility] — standard: [measurable bar]."
- "This isn't a project — it's an ongoing area. What's the standard we're holding it to?"
- "Which of my areas does this belong to?"

---

## Resources: Detailed Guide

### The Interest Test

Resources should reflect genuine, active interests — not aspirational ones. The test: "Have I engaged with material on this topic in the last 90 days?" If not, it belongs in Archives.

### Resource Hygiene

| Signal | Diagnosis | Action |
|--------|-----------|--------|
| You have 50+ resource topics | You're collecting, not curating | Archive everything you haven't touched in 90 days |
| Resources folder is your largest category | You're saving "just in case" instead of "just in time" | Apply the three capture criteria more strictly |
| You never pull from Resources into Projects | Resources aren't connected to your actual work | Either your interests and projects are misaligned, or your organization makes retrieval too hard |
| Resource notes are all Layer 1 (raw captures) | You're stockpiling, not learning | Apply progressive summarization to the 10 most relevant resource notes |

### Resources for PMs: Common Topics

- Product-led growth strategies
- Pricing and monetization models
- Platform and ecosystem thinking
- Organizational design for product teams
- Data science and analytics methods
- Industry-specific domain knowledge
- Leadership and management frameworks
- Technical architecture patterns
- Behavioral psychology and user research methods
- Go-to-market strategies

### Product Applications

| Context | Application | Example |
|---------|-------------|---------|
| Career development | Resources reflect your intellectual interests and growth edges | A PM interested in transitioning to platform PM keeps a "Platform Thinking" resource |
| Innovation inputs | Resources become project inputs when the timing is right | "API-first architecture" resource feeds the next platform strategy project |
| Mentoring | Share curated resource collections with junior PMs | "Here's my 'Stakeholder Management' resource — the distilled highlights from 15 articles and 3 books" |

### Copy Patterns

- "This is interesting but not tied to any active project — file it as a Resource and move on."
- "Pull the Resource on [topic] into the project folder; that's where it'll actually get used."
- "If I'm not genuinely interested in this anymore, it goes to Archives."

---

## Archives: Detailed Guide

### The Kitchen Cleanup Metaphor

Forte's Kitchen Cleanup metaphor: organize by activity, not taxonomy. What you're cooking now is on the counter (Projects), staples are at eye level (Areas), specialty ingredients on higher shelves (Resources), expired or seasonal items in storage (Archives). Archives are not a trash can — they're a knowledge reserve, and the first place to look when starting a new project is the Archive of similar past projects. That's where compounding knowledge actually lives.

### What Goes to Archives

| Source | Trigger for Archiving | What to Extract First |
|--------|----------------------|----------------------|
| Completed projects | Project goal achieved or abandoned | Intermediate packets: key deliverables, analyses, templates |
| Changed responsibilities | Role change, reorg, or delegation | Handoff document; standard definitions for the successor |
| Dropped interests | No engagement in 90+ days | Nothing — just move it |
| Outdated reference material | Information superseded by newer sources | Update the relevant Area or Resource with current material first |

### The Archive-Don't-Delete Principle

Never delete material from your Second Brain — archive it. Storage is essentially free. The cost of re-creating a deleted analysis or re-finding a deleted reference far exceeds the cost of keeping it searchable in Archives. The only exceptions are information that's genuinely sensitive and should not persist (credentials, terminated employment agreements, etc.).

### Retrieval from Archives

Archives should be organized enough that you can find past material when a new project makes it relevant. The retrieval path:

1. **Search** — Most note-taking tools have search that covers archived material
2. **Browse by project name** — If you remember the project, navigate to its archived folder
3. **Progressive summarization** — Layer 4 summaries on key archived notes make scanning fast

### Product Applications

| Context | Application | Example |
|---------|-------------|---------|
| Retrospectives | Archive the project folder with retro notes included | Future PMs running similar projects can review what worked and what didn't |
| Pattern recognition | Review Archives when starting similar projects | Before a new pricing project, review the archived "Q3 Pricing Restructure" folder |
| Audit trail | Archives provide decision history for compliance or leadership questions | "Why did we choose approach X?" — the archived project folder has the analysis and decision memo |

### Copy Patterns

- "Before I start, let me check Archives for a similar past project."
- "This project is done — archive the folder and extract the reusable packets first."
- "I haven't touched this in months; archive it and trust I can search later."

---

## PARA and Product Team Artifacts

| Artifact | PARA Category | Lifecycle |
|----------|--------------|-----------|
| PRD | Project → Archive | Created for a specific project; archived when shipped |
| Product strategy memo | Project → Archive (or Area if it's a living document) | Created quarterly; archived when superseded |
| Customer interview notes | Project (if for a specific initiative) or Area (if ongoing) | Active during research; archived when synthesized |
| Competitive analysis | Project (if for a deliverable) or Area (if maintained ongoing) | Depends on whether competitive awareness is an area or a one-time project |
| OKR documents | Project (quarterly cycle) → Archive | Created quarterly; archived at quarter end |
| Team retrospective notes | Area: "Team Operations" → Archive after action items complete | Ongoing area artifact |
| Technical architecture docs | Area: "Technical Architecture" | Living document; updated as architecture evolves |
| Onboarding materials | Area: "Team Operations" | Living artifact; updated as processes change |
| Conference notes | Resource or Project | Resource if general interest; Project if feeding a specific initiative |

---

## Cross-Role Examples

### IC PM Organizing a Product Launch

```
PROJECTS
├── Q2 Feature Launch (deadline: June 1)
├── Pricing Page Redesign (deadline: May 15)
├── User Research: Activation Flow (deadline: April 30)

AREAS
├── Product Quality
├── Stakeholder Relationships
├── Customer Research Practice

RESOURCES
├── Behavioral Psychology in Product
├── Pricing Strategies
├── Competitor Strategies

ARCHIVES
├── [Completed] Q1 Onboarding Redesign
├── [Completed] 2024 Annual Planning
├── [Dropped] Internal Tooling Investigation
```

### Group PM / Director Organizing a Portfolio

```
PROJECTS
├── Annual Planning 2025 (deadline: December 15)
├── Hire PM for Platform Team (deadline: January 31)
├── Board Presentation: Product Strategy (deadline: February 10)

AREAS
├── Portfolio Strategy
├── Team Development (4 direct reports)
├── Executive Stakeholder Relationships
├── Hiring Pipeline
├── Cross-Team Coordination

RESOURCES
├── Product Leadership Frameworks
├── Organizational Design
├── Industry Trends: [Your Vertical]

ARCHIVES
├── [Completed] 2024 Reorg Planning
├── [Completed] Q4 Board Presentation
├── [Former Report] PM Development Plans (handed off)
```

---

## Summary: The Categorization Flowchart

For any piece of information, run through this sequence:

1. **Is it connected to a current project?** → Put it in that project's folder.
2. **Is it related to an ongoing area of responsibility?** → Put it in that area's folder.
3. **Is it a topic of genuine active interest?** → Put it in the relevant resource topic.
4. **Is it none of the above?** → Don't save it. Or if it was previously in your system, archive it.

The most common error is skipping step 1. Information that's relevant to an active project should go in that project's folder — even if it "belongs" to a topic. Actionability trumps taxonomy.
