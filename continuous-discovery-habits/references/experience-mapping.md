# Experience Mapping

Experience maps are visual artifacts that capture how a customer accomplishes a goal today — step by step, with the actions they take, the thoughts running through their head, and the emotions they feel along the way. They are built collaboratively from interview data, and they generate opportunities you would never discover by brainstorming in a conference room. This guide covers how to construct, use, and avoid common pitfalls with experience maps in continuous discovery.

## Why Map the Current State, Not the Future

Most product teams skip directly to future-state journey maps — "imagine if our product worked like this" — and miss the entire point. The current-state experience map is upstream of every future design decision because it reveals:

- **Workarounds you would not invent.** Customers patch over your product's gaps with their own ingenuity. Those patches are evidence of unmet needs.
- **Emotional friction your data cannot see.** Click-tracking shows what users do, not how they feel. A user can complete a flow successfully and still hate every minute of it.
- **The full context outside your product.** Customers do not live inside your tool. Their experience includes Excel, Slack, phone calls, and their boss's expectations. Map the whole thing.
- **Hidden steps that block adoption.** "I have to ask Finance first" or "I wait until Marco gets back from lunch" are invisible to your product analytics and impossible to brainstorm without interviews.

A future-state map without a grounded current-state map produces optimistic, internally satisfying fiction. Teams ship features for users who do not exist.

## Experience Maps vs. Journey Maps

These terms are used interchangeably but mean different things:

| Artifact | Scope | Purpose |
|----------|-------|---------|
| **Journey map** | Touchpoints with your product or company | Optimize your product's specific user experience |
| **Experience map** | The customer's full goal-accomplishment, regardless of which tools they use | Discover unmet needs that may live outside your product |

Continuous discovery favors experience maps because the most valuable opportunities often hide in the gaps *between* tools, not inside your own.

## The Four Layers of an Experience Map

Every step on an experience map has four layers stacked vertically. Map them in this order, top to bottom:

| Layer | Question | Source |
|-------|----------|--------|
| **1. Phase** | What stage of the goal are they in? (e.g., "Researching," "Negotiating," "Implementing") | Synthesis of multiple interviews |
| **2. Actions** | What do they actually do at this step? | Direct interview reports |
| **3. Thoughts** | What is going through their head? | Direct quotes from interviews |
| **4. Emotions** | How do they feel? Where are the high and low points? | Tone, body language, words like "frustrating," "relieved," "stressed" |

The emotional layer is the most undervalued. It is also the layer most likely to reveal opportunities. Peaks of high frustration or anxiety are opportunity hotspots.

## Step-by-Step Construction

### Step 1: Define the Map's Boundaries

Before drawing anything, agree on three things:

1. **Whose experience is this?** Be specific. Not "customers" — "hiring managers at Series A SaaS companies, 50-200 employees, who own at least one open role per quarter."
2. **What goal are they trying to accomplish?** Frame as a complete outcome from the customer's perspective. "Hire a senior engineer" — not "Use our ATS."
3. **What is the start and end point?** "Starts when the headcount is approved. Ends when the candidate signs an offer."

Without these boundaries, the map sprawls into uselessness.

### Step 2: Pull Steps from Interview Transcripts

Re-read your interview transcripts with a single question in mind: *what did they do, in what order, to accomplish this goal?* Extract each discrete action as a sticky note (literal or digital). Do not synthesize yet — capture raw steps from each interview separately.

Common raw steps for the hiring manager example might be:

- "Got the headcount approved by my VP"
- "Drafted a job description in Google Docs"
- "Sent the JD to the recruiter via Slack"
- "Waited 3 weeks for the first batch of candidates"
- "Reviewed resumes on Sunday morning while making coffee"
- "Argued with the recruiter about screening criteria"
- "Set up a 4-person interview panel via Calendly"

### Step 3: Merge and Sequence

Lay out steps from all interviews. Merge duplicates. Sequence them along a horizontal axis. The first version will be messy — that is fine.

Pay particular attention to **branches and loops**: do all customers follow the same path, or are there forks? Loops (where the user repeats steps) are often signals of friction.

### Step 4: Layer in Thoughts and Emotions

For each step, pull a direct quote from your interviews that captures what the customer was thinking or feeling. Use actual customer language. If you cannot find a quote for a step, that is a signal you need another interview before the map is complete.

Plot emotions on a simple curve below the actions:

```
Excited   *
Neutral   --*-----*-------*------*---*
Anxious        *           *
Frustrated              *           *
              ↑           ↑
        First batch    Reviewed
        of candidates  resumes Sunday
```

The low points are where opportunities live.

### Step 5: Annotate Pain Points and Workarounds

Mark every step that includes a pain point or a workaround. These are the candidate opportunities you will lift onto the Opportunity Solution Tree.

| Symbol | Meaning |
|--------|---------|
| 🔴 | Pain point — customer experiences friction, failure, or frustration |
| 🟡 | Workaround — customer hacks their way around an obstacle |
| 🔵 | Unmet need — customer wishes something existed but does not articulate it as a feature |

## From Map to OST: Lifting Opportunities

Once the map is annotated, each red, yellow, or blue marker becomes a candidate opportunity for the OST. Restate each marker as an opportunity statement using the format from `opportunity-discovery.md`:

> "[Customer segment] needs a way to [do something] so that [desired outcome], but today [current obstacle]."

Example lift from the hiring manager map:

| Map marker | Opportunity statement |
|------------|----------------------|
| 🔴 "Reviewed resumes on Sunday morning while making coffee" | Hiring managers need a way to triage candidates within their workweek so that they can maintain work-life boundaries, but today resumes arrive in batches that force weekend work. |
| 🟡 "Set up a 4-person interview panel via Calendly" | Hiring managers need a way to coordinate panel interviews without leaving the ATS so that they avoid managing scheduling in a separate tool, but today they bridge two systems manually. |
| 🔵 "Wished I had more control over screening criteria" | Hiring managers need a way to define and adjust screening criteria collaboratively with the recruiter so that they trust the candidate pipeline, but today they delegate criteria entirely and lose confidence in the results. |

Not every marker becomes a top-priority opportunity. Run them through the prioritization framework in `prioritization-methods.md` to decide which deserve solutions.

## Running a Collaborative Mapping Workshop

Experience maps work best when built collaboratively with the full product trio. A 3-hour workshop produces a richer artifact and a shared understanding that survives long after the meeting.

### Workshop Structure

| Time | Activity | Output |
|------|----------|--------|
| 0:00–0:15 | Frame the map: who, what goal, start/end | Boundaries agreed |
| 0:15–0:45 | Each person reads 1-2 interview transcripts, captures raw steps on sticky notes | Pile of raw steps |
| 0:45–1:15 | Merge and sequence steps as a group | Draft horizontal map |
| 1:15–2:00 | Add thought and emotion layers | Four-layer map |
| 2:00–2:30 | Mark pain points, workarounds, unmet needs | Annotated map |
| 2:30–3:00 | Lift candidate opportunities onto the OST | Opportunity list ready for prioritization |

Each participant must come to the workshop having read interview transcripts. Skipping the pre-read produces maps based on assumption rather than evidence.

### Tools

- **Physical:** sticky notes, large wall space, markers. Highest engagement.
- **Digital:** Miro, FigJam, Mural. Necessary for distributed teams. Use templates with the four-layer structure pre-drawn.
- **Database:** Notion, Airtable. Good for keeping the map alive over months but worse for the live workshop.

## Common Mapping Mistakes

### Mistake 1: Mapping What You Wish Customers Did

Teams unconsciously map the experience they want to design, not the one customers actually have today. Watch for steps that sound like "User logs in and is delighted by the dashboard" — that is fiction.

**Fix:** For every step, point to the interview quote that supports it. If you cannot, remove the step or interview more customers.

### Mistake 2: Mapping Only the Happy Path

A map that shows only the successful flow misses the most valuable opportunities. The customers who churn, who abandon onboarding, who silently work around your gaps — those are the ones whose maps reveal the biggest unmet needs.

**Fix:** Deliberately interview customers who failed or struggled. Build a separate "unhappy path" map and compare.

### Mistake 3: Building the Map Without the Engineers

If only PMs and designers build the map, engineering inherits decisions they did not participate in shaping. They also miss the rich context that makes feasibility judgments easier later.

**Fix:** The full trio attends. If a tech lead cannot attend, postpone the workshop.

### Mistake 4: Finishing the Map and Filing It

Experience maps are living artifacts, not deliverables. A map built six months ago describes a customer experience that no longer exists.

**Fix:** Treat the map as a working document. Update it as new interview data accumulates. Display it visibly so the team sees it daily.

### Mistake 5: Mapping Inside Your Product Boundary

The most powerful insights come from the parts of the experience that happen outside your product. If your map starts at "user opens the app" and ends at "user closes the app," you are missing the upstream and downstream context that determines whether your product matters in the first place.

**Fix:** Extend the map at both ends. What happened *before* they opened your app? What did they need to do *after* closing it? The gaps in between are where opportunities live.

## Summary

Experience mapping turns interview data into a shared, visual model of the customer's reality. It exposes pain points and workarounds invisible from inside the product, surfaces emotional friction that analytics cannot measure, and generates opportunities for the Opportunity Solution Tree that no brainstorming session can match. Build maps collaboratively with the full trio, ground every step in interview evidence, and update the artifact continuously as understanding deepens.
