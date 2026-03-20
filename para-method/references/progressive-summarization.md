# Progressive Summarization

Progressive Summarization is Forte's technique for making notes retrievable without requiring full re-reading. It creates a gradient from detailed source material to compressed core insight, applied incrementally over time as a note proves its usefulness. The key insight is that you never summarize a note "just in case" — you summarize it when you have a reason to revisit it, which means the most useful notes naturally receive the most distillation.

---

## The Problem Progressive Summarization Solves

Knowledge workers face a fundamental tension:

- **Capture too much detail** and notes become unreadable walls of text. Retrieval requires re-reading the entire note, which takes nearly as long as finding the original source.
- **Capture too little detail** and notes lose their context. A bullet point that says "interesting pricing insight" is useless six months later when you can't remember what the insight was.

Progressive Summarization resolves this by keeping all the detail while layering increasingly compressed summaries on top. You choose your depth of engagement based on your current need:

- Need the full context? Read the entire note (Layer 1).
- Need the key points quickly? Scan the bold passages (Layer 2).
- Need the core insight in 10 seconds? Read the highlights (Layer 3).
- Need a one-line reminder of what this note contains? Read the executive summary (Layer 4).

---

## The Five Layers in Detail

### Layer 0: Original Source

The unmodified source material — an article, a transcript, a document. This lives outside your Second Brain in most cases (the original website, the original PDF, the Slack thread). Your Second Brain doesn't need to contain copies of everything; it contains your processed versions.

### Layer 1: Captured Notes

Your initial save — the first act of selection. By choosing what to capture, you've already filtered out most of the source material.

**What Layer 1 looks like:**
- Book highlights exported from your reading app
- Meeting notes taken during a conversation
- Interview transcript excerpts you selected
- Article passages you copied into your notes

**PM example — Customer Interview:**
```
Layer 1: Captured Notes
---
Customer: Sarah, VP Operations, Acme Corp (200 employees)
Date: 2025-01-15

"We tried three different tools before settling on spreadsheets.
The problem isn't features — every tool had enough features. The
problem is that nobody on my team has time to learn a new system
when the spreadsheet already works."

"Our biggest pain isn't the data entry. It's that I can't get a
real-time picture of where things stand. I have to ask three
people and wait for them to update the sheet."

"We'd switch tomorrow if onboarding took less than a day. We
tried [Competitor] and the implementation was quoted at 6 weeks.
That's not realistic for us."

My observation: Strong signal that implementation speed is the
real differentiator, not feature depth. This contradicts our
assumption that we need to match Competitor's feature set.
```

### Layer 2: Bold Passages

On a second read — typically when the note becomes relevant to an active project — you bold the passages that stand out as most important.

**When to apply Layer 2:**
- You're pulling this note into an active project folder
- You're reviewing notes for a specific decision
- You revisit a note and want to mark what matters most

**PM example — Same note with Layer 2 applied:**
```
Layer 2: Bold Passages Added
---
Customer: Sarah, VP Operations, Acme Corp (200 employees)
Date: 2025-01-15

"We tried three different tools before settling on spreadsheets.
**The problem isn't features — every tool had enough features.
The problem is that nobody on my team has time to learn a new
system** when the spreadsheet already works."

"Our biggest pain isn't the data entry. **It's that I can't get
a real-time picture of where things stand.** I have to ask three
people and wait for them to update the sheet."

**"We'd switch tomorrow if onboarding took less than a day.**
We tried [Competitor] and the implementation was quoted at 6
weeks. That's not realistic for us."

My observation: **Strong signal that implementation speed is the
real differentiator, not feature depth.** This contradicts our
assumption that we need to match Competitor's feature set.
```

### Layer 3: Highlighted Passages

Within the bold, highlight the absolute core — the sentences that capture the essential insight. This is the layer where you could scan the note in 10-15 seconds and get the key takeaway.

**When to apply Layer 3:**
- The note is actively informing a decision you're making right now
- You want to make this note instantly scannable for future retrieval
- You're preparing to use this note in a deliverable

**PM example — Same note with Layer 3:**
```
Layer 3: Highlights Within Bold
---
(Bold shown in **, highlights shown in ==)

**==The problem isn't features — every tool had enough features.==**

**==I can't get a real-time picture of where things stand.==**

**==We'd switch tomorrow if onboarding took less than a day.==**

**==Implementation speed is the real differentiator, not
feature depth.==**
```

### Layer 4: Executive Summary

A 2-3 sentence summary written in your own words, placed at the top of the note. This is the layer that transforms a note from a record into an insight. Writing the summary forces you to synthesize what you've learned.

**When to apply Layer 4:**
- The note has proven useful across multiple projects
- You want to make retrieval instant — future you can read 2 sentences instead of scanning the full note
- You're extracting this as an Intermediate Packet

**PM example — Same note with Layer 4:**
```
Layer 4: Executive Summary
---
SUMMARY: Mid-market buyers (200 employees) don't need more
features — they need faster implementation. Onboarding speed
under 1 day is the primary switching trigger. Deprioritize
feature parity with competitors; prioritize time-to-value.

[Full note with bold and highlights below...]
```

### Layer 5: Remix

The note's insights are combined with other notes to produce new creative output. This is the Express step of CODE. Layer 5 doesn't modify the original note — it uses the distilled material as input for a new deliverable.

**PM example — Layer 5 output:**
A section in a strategy memo that synthesizes this interview with three others:

```
"Our customer research reveals a consistent pattern across
mid-market buyers: implementation speed, not feature depth,
is the primary differentiator. Four of our seven mid-market
interviews cited onboarding time as their top switching
criterion, with the threshold at 1 day or less. This
directly challenges our current roadmap, which prioritizes
feature parity with [Competitor]. Recommendation: shift
Q2 investment from [Feature X] to reducing onboarding
time from 2 weeks to 1 day."
```

---

## When to Apply Each Layer: Decision Guide

| Situation | Layer to Apply | Time Investment |
|-----------|---------------|-----------------|
| First capture | Layer 1 only | 2-5 minutes |
| Note surfaces during project search | Layer 2 (bold key passages) | 3-5 minutes |
| Using note for an active decision | Layer 3 (highlight within bold) | 2-3 minutes |
| Note has been useful 3+ times | Layer 4 (executive summary) | 3-5 minutes |
| Producing a deliverable | Layer 5 (remix into output) | Varies |
| Weekly Review — processing inbox | Layer 1 for new captures | 1-2 min per note |
| Monthly Review — deepening key notes | Layer 2-3 for notes used this month | 15-20 min total |

**The critical principle:** Most notes will never go beyond Layer 1 or 2. That is correct and expected. Only 10-20% of your notes will reach Layer 3. Only 5-10% will reach Layer 4. This is not a failure — it's the system working as designed, directing your distillation effort toward the material that has proven most valuable.

---

## Progressive Summarization for PM Artifacts

### Customer Interview Notes

| Layer | What It Contains | Retrieval Use Case |
|-------|-----------------|-------------------|
| 1 | Full interview notes with quotes and observations | Deep context when revisiting the customer's situation |
| 2 | Bold: key quotes and surprising observations | Scanning during synthesis across multiple interviews |
| 3 | Highlight: the one or two core insights | Quick reference when building an opportunity solution tree |
| 4 | Summary: "This customer's core need is X; primary switching criterion is Y" | Instant pattern matching across many interview notes |

### Competitive Analysis Notes

| Layer | What It Contains | Retrieval Use Case |
|-------|-----------------|-------------------|
| 1 | Full analysis: features, pricing, positioning, strengths, weaknesses | Deep reference during competitive positioning work |
| 2 | Bold: unique differentiators and notable gaps | Quick comparison during roadmap prioritization |
| 3 | Highlight: the competitive insight that most affects your strategy | Scanning when preparing stakeholder presentations |
| 4 | Summary: "Competitor X's key advantage is A; our counter-positioning is B" | Instant recall during conversations with executives or customers |

### Book and Article Notes

| Layer | What It Contains | Retrieval Use Case |
|-------|-----------------|-------------------|
| 1 | Highlights and annotations from reading | Revisiting when a project makes the book relevant |
| 2 | Bold: frameworks and examples most applicable to your work | Scanning when looking for a framework to apply |
| 3 | Highlight: the single most useful concept or model | Quick retrieval of the key idea |
| 4 | Summary: "This book's core argument is X; most useful framework is Y; apply when Z" | Deciding whether to revisit the full notes |

---

## Common Mistakes in Progressive Summarization

| Mistake | Why It Fails | Fix |
|---------|-------------|-----|
| Summarizing every note to Layer 4 immediately | Wasted effort on notes you may never revisit; creates a chore instead of a practice | Only apply Layer 2+ when you have a reason to revisit |
| Bolding too much (more than 30% of the text) | If everything is bold, nothing is bold; defeats the purpose of visual scanning | Aim for 10-20% of the text in bold at Layer 2 |
| Highlighting too much (more than 20% of the bold) | Same problem one level deeper | Aim for the smallest possible highlighted set that captures the core insight |
| Skipping Layer 4 and going straight to Layer 5 | You lose the intermediate step of synthesis; your output becomes a patchwork of quotes instead of original thinking | Write the summary first; the act of summarizing in your own words is where insight happens |
| Using progressive summarization on notes that don't need it | Not every note needs distillation; meeting logistics, action items, and transient information can stay at Layer 1 | Apply only to notes that contain insights, not to notes that contain tasks or logistics |
| Never reaching Layer 5 | The system captures and distills but never produces output; knowledge doesn't become work product | For every major deliverable, deliberately pull from distilled notes; make assembly the default mode |

---

## Summary

Progressive Summarization is a demand-driven distillation system. You invest summarization effort in proportion to a note's demonstrated value. Layer 1 is cheap and universal. Each subsequent layer costs more attention but makes retrieval faster. Most notes stay at Layer 1-2. The few that reach Layer 3-4 become your most valuable intellectual assets — instantly retrievable, densely compressed, and ready to fuel creative output. The practice works because it aligns effort with value: you distill what you use, not what you might use.
