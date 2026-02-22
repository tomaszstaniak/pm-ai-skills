# Opportunity Discovery

Opportunities are unmet customer needs, pain points, and desires. They live in the space between what customers want to accomplish and what they can accomplish today. This guide covers how to uncover opportunities through story-based interviews, extract and organize them into a useful structure, and prioritize which ones to pursue.

## Story-Based Interview Techniques

The goal of a customer interview is not to ask people what they want. It is to understand what they actually do, what gets in their way, and what matters to them. Story-based interviewing achieves this by grounding every question in a specific, real past event.

### The Core Technique: "Tell Me About the Last Time..."

The single most powerful interview prompt is a request for a specific story:

- "Tell me about the last time you tried to [activity related to your product outcome]."
- "Walk me through what happened the last time you [relevant task]."
- "Think about the most recent time you [situation]. What happened?"

This prompt works because:

1. **It anchors in reality.** People reconstruct actual events rather than speculating about hypothetical behavior.
2. **It surfaces details they would not volunteer.** The narrative structure pulls out context, workarounds, emotions, and decision points.
3. **It bypasses rationalization.** People are unreliable reporters of their own preferences but accurate reporters of what happened yesterday.

### The Interview Flow

A well-structured interview follows this arc:

**Opening (2-3 minutes)**
Build rapport. Explain that you are here to learn, not to sell. Set expectations: "There are no right or wrong answers. I want to hear about your real experience."

**Story Elicitation (15-20 minutes)**
Ask for a specific recent story. Then follow the story wherever it goes, using these follow-up techniques:

| Technique | Example | Purpose |
|-----------|---------|---------|
| **Temporal probing** | "What happened next?" / "What did you do before that?" | Reconstruct the full sequence of events |
| **Emotional probing** | "How did that feel?" / "What was frustrating about that?" | Uncover pain points and motivation |
| **Decision probing** | "What made you choose that option?" / "What else did you consider?" | Reveal decision criteria and alternatives |
| **Workaround probing** | "How do you handle that today?" / "What do you do when that happens?" | Find unmet needs being solved with hacks |
| **Context probing** | "Who else was involved?" / "Where were you when this happened?" | Understand the full situation |
| **Frequency probing** | "How often does that happen?" / "When was the last time before that?" | Assess severity and frequency |

**Broadening (5-10 minutes)**
After the first story, ask for related stories: "Can you think of another time when something similar happened?" or "What about a time when it went really well — what was different?"

**Closing (2-3 minutes)**
Ask if there is anything else they want to share. Thank them. Do not pitch your product or ideas.

### What Not to Do

**Never ask "Would you use X?"** Hypothetical usage questions produce hypothetical answers. People say yes to be polite, to seem progressive, or because they genuinely believe they would — but belief and behavior diverge wildly.

**Never ask "What would you like us to build?"** Customers are experts on their problems, not on solutions. Henry Ford's apocryphal quote about faster horses captures this perfectly. Your job is to understand the need; the team's job is to design the solution.

**Never ask leading questions.** "Don't you think it would be easier if...?" tells the interviewee what you want to hear. Replace with: "How easy or difficult was that for you?"

**Never fill silence.** When the interviewee pauses, wait. They are often about to say something important. Count to seven in your head before speaking.

**Never interview in groups.** Group dynamics introduce conformity bias. One person shares an opinion and others adjust theirs. Always interview one-on-one.

## The Interview Snapshot

After each interview, create an Interview Snapshot — a structured one-page summary that makes the interview findable, shareable, and useful for synthesis.

### Interview Snapshot Template

```
INTERVIEW SNAPSHOT

Date:           [Date of interview]
Participant:    [Anonymized identifier, e.g., "P12 — Marketing Manager, mid-market SaaS"]
Interviewer:    [Name]
Product Outcome: [The outcome this interview relates to]

QUICK FACTS
- Role/title:
- Company size:
- How long using [product/category]:
- Key tools mentioned:

STORY SUMMARY
[2-3 sentence summary of the main story they told.
What were they trying to do? What happened? How did it end?]

OPPORTUNITIES IDENTIFIED
1. [Opportunity: unmet need or pain point, stated in customer language]
2. [Opportunity]
3. [Opportunity]

KEY QUOTES
- "[Direct quote that captures a pain point or insight]"
- "[Direct quote]"

SURPRISES
[Anything unexpected that challenges your assumptions or opens a new line of inquiry]

FOLLOW-UP
[Questions this interview raised that you want to explore in future interviews]
```

### Tips for Good Snapshots

- Write the snapshot within 30 minutes of the interview, while memory is fresh.
- Use the customer's language, not your internal jargon.
- Each opportunity should be a need or pain point, not a feature request. If the customer said "I wish you had a Gantt chart," the opportunity is "Needs to visualize task dependencies and timelines across the team" — the underlying need, not the stated solution.
- Limit to 3-5 opportunities per interview. If you identified more, prioritize the ones most connected to your product outcome.

## Extracting Opportunities from Interview Transcripts

If you record and transcribe interviews, use this process to extract opportunities systematically.

### Step 1: Highlight Signals

Read through the transcript and highlight any statement that reveals:
- A pain point ("This is really frustrating because...")
- A workaround ("What I usually do is...")
- A desire ("I wish I could...")
- A constraint ("The problem is that...")
- An unmet goal ("I was trying to... but...")
- A moment of confusion ("I wasn't sure how to...")
- An emotional reaction ("That drives me crazy" / "I love when...")

### Step 2: Rewrite as Opportunity Statements

Convert each highlighted signal into a neutral opportunity statement. Use this format:

**"[Customer segment] needs a way to [do something] so that [desired outcome], but today [current obstacle]."**

Examples:

| Raw Interview Quote | Opportunity Statement |
|----|-----|
| "I spend like two hours every Monday just copying numbers from Salesforce into our spreadsheet." | Sales managers need a way to consolidate pipeline data from multiple sources without manual effort so that they can spend Monday mornings on strategy instead of data entry. |
| "I never know if my teammate already responded to that customer or not." | Support agents need a way to see real-time teammate activity on a ticket so that they avoid duplicate responses and conflicting information. |
| "I tried to set up the integration but I got some error and just gave up." | New users need a way to complete integrations without encountering blocking errors so that they reach value quickly and do not abandon setup. |

### Step 3: De-duplicate

After processing multiple interviews, you will find overlapping opportunities. Merge duplicates, keeping the version that is most clearly stated and broadest without being vague.

## Building Opportunity Hierarchies

A flat list of opportunities becomes unmanageable after 5-10 interviews. The Opportunity Solution Tree uses a hierarchical structure to organize them.

### Parent and Child Opportunities

A **parent opportunity** is a broad need area. **Child opportunities** are specific manifestations of that need.

Example hierarchy:

```
Product Outcome: Increase % of new users who reach first value moment within 48 hours

├── Opportunity: New users struggle to understand what the product does
│   ├── Landing page messaging does not match their mental model
│   ├── No guided tour or suggested first action after signup
│   └── Feature names use internal jargon instead of user language
│
├── Opportunity: New users cannot connect their existing tools
│   ├── Integration setup requires technical knowledge users do not have
│   ├── Error messages during setup are unhelpful
│   └── Users do not know which integrations are available
│
└── Opportunity: New users do not see value until teammates join
    ├── Invitation flow is buried in settings
    ├── Product feels empty with only one user's data
    └── No way to demonstrate value to teammates before they join
```

### Rules for Good Hierarchies

1. **Parent opportunities should be broad enough to contain multiple children** but narrow enough to be clearly distinct from sibling parents.
2. **Child opportunities should be specific enough to suggest solution directions** but still framed as needs, not solutions.
3. **No more than 3-5 parent opportunities per product outcome.** If you have more, some parents are likely children of a higher-level parent.
4. **Update the hierarchy weekly** as new interview data comes in. Opportunities move, merge, split, and get re-prioritized.
5. **The hierarchy is a living artifact.** It is not a deliverable to be finalized — it is a thinking tool that evolves continuously.

## Prioritizing Opportunities

Not all opportunities are worth pursuing. Use a structured framework to decide which opportunities to explore for solutions.

### The Frequency x Severity x Outcome Alignment Framework

Score each opportunity on three dimensions:

| Dimension | Question | Scale |
|-----------|----------|-------|
| **Frequency** | How often do customers encounter this problem? | 1 (rarely) to 5 (daily or more) |
| **Severity** | How painful is it when they encounter it? | 1 (minor annoyance) to 5 (blocking, causes failure) |
| **Outcome Alignment** | How directly does solving this connect to our product outcome? | 1 (loosely related) to 5 (directly drives the metric) |

Multiply the three scores to get a priority score (max 125). This is a heuristic, not a formula — use it to facilitate discussion, not to make decisions by spreadsheet.

### Prioritization Table Example

| Opportunity | Freq | Sev | Align | Score | Notes |
|------------|------|-----|-------|-------|-------|
| Integration setup requires technical knowledge | 4 | 5 | 5 | 100 | Blocks first value moment entirely |
| No guided tour after signup | 5 | 3 | 4 | 60 | High frequency but users find workarounds |
| Feature names use internal jargon | 3 | 2 | 3 | 18 | Real but lower impact |
| Product feels empty with one user | 4 | 4 | 5 | 80 | Strong alignment with collaborative value |
| Invitation flow is buried | 3 | 3 | 4 | 36 | Easy fix, moderate impact |

### Additional Prioritization Considerations

Beyond the scoring framework, consider:

- **Number of interviews where this opportunity appeared.** An opportunity mentioned by 8 of 10 interviewees is more validated than one mentioned by 2 of 10.
- **Segment concentration.** Does this opportunity cluster in a specific customer segment? If so, is that segment strategically important?
- **Existing momentum.** Is the team already close to this problem space? Sometimes an opportunity that scores slightly lower is worth pursuing because you already have context, data, and partially built solutions.
- **Dependencies.** Some opportunities cannot be solved until others are addressed first. Map these dependencies before committing to a sequence.

## Common Interviewing Mistakes

### Mistake 1: Interviewing Only Power Users

Power users are the easiest to recruit and the most willing to talk. But they have already overcome the obstacles that block most people. If your product outcome relates to activation or onboarding, you need to talk to people who struggled, churned, or never got started.

**Fix:** Deliberately recruit across the experience spectrum. Interview recent signups, lapsed users, and people who evaluated your product but chose a competitor.

### Mistake 2: Asking About the Future

"How would you use this feature?" and "Would this solve your problem?" generate fiction, not data. People cannot predict their own behavior reliably.

**Fix:** Stay in the past. "Tell me about the last time you encountered this problem" is always more reliable than "Imagine if you had this tool."

### Mistake 3: Interviewing Too Infrequently

One round of interviews before a big project is not continuous discovery. Insights decay. Markets shift. New patterns emerge. A single interview sprint creates a snapshot that goes stale within weeks.

**Fix:** Conduct at least one customer interview per week, every week, indefinitely. This is the core habit. It does not require elaborate scheduling — even 20-minute conversations yield usable insights when conducted consistently.

### Mistake 4: Not Connecting Interviews to Outcomes

Interviews without a product outcome produce interesting but unfocused stories. You learn things but cannot act on them because they do not connect to what your team is trying to achieve.

**Fix:** Start every interview by reviewing your product outcome. Frame your opening question around the behavior you are trying to change. Filter opportunities through outcome alignment.

### Mistake 5: Taking Notes Instead of Listening

When you are writing furiously, you miss body language, emotional cues, and follow-up opportunities. The conversation becomes an extraction exercise rather than a genuine exchange.

**Fix:** Record interviews (with permission) and take minimal notes — just enough to capture key moments. Write the full Interview Snapshot afterward using the recording.

### Mistake 6: Treating Interview Insights as Certainty

One customer saying something does not make it true for all customers. Three customers saying the same thing is a pattern worth investigating, not a fact to build on.

**Fix:** Track how many interviews surface each opportunity. Look for convergence across multiple participants before elevating an opportunity to high priority. Use the opportunity hierarchy to aggregate evidence over time.

## Weekly Interview Cadence

Teresa Torres recommends that the product trio (product manager, designer, tech lead) conducts at least one interview per week. Here is a practical weekly rhythm:

| Day | Activity |
|-----|----------|
| **Monday** | Review current opportunity tree. Identify gaps. Decide what to probe this week. |
| **Tuesday-Wednesday** | Conduct 1-2 interviews (30 minutes each). |
| **Thursday** | Write Interview Snapshots. Extract opportunities. Update the opportunity tree. |
| **Friday** | Trio reviews updated tree. Reprioritize if needed. Decide next interview focus. |

This cadence turns customer understanding from a periodic event into a continuous practice. Over a quarter, 12-24 interviews generate a rich, evolving map of the opportunity space that no amount of stakeholder brainstorming can replicate.

## Summary

Opportunity discovery is the practice of systematically uncovering and organizing customer needs. Story-based interviews ground your understanding in real behavior rather than opinion. Interview Snapshots make insights durable and shareable. Opportunity hierarchies give structure to a growing body of evidence. Prioritization ensures you focus on the opportunities most likely to drive your product outcome. And a weekly cadence ensures the practice is continuous, not episodic.
