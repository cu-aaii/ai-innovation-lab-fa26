# A2 — Weekly 4-Box Report

!!! abstract "Submission details"
    **Type:** Team · **Weight:** 20% of final grade  
    **Due:** Every Friday by 5:00 PM ET (best 10 of 12 count)  
    **Format:** Text entry on Canvas (no file upload)  
    **Where:** Canvas → Assignments → Weekly 4-Box (Week #)

---

## Overview

The 4-Box is your team's weekly status report. It is the working artifact your stakeholders, Tech Lead, and TA use to understand where the project is each week: what you committed to, what you shipped, and what's at risk.

A good 4-Box is **short, specific, and honest.** Treat this as the document a busy stakeholder would read in 90 seconds and walk away with an accurate picture of your team's status.

**Best 10 of 12 count.** Each week is authored by a rotating team member — over 12 weeks, every team member should have authored at least 2–3 reports.

---

## Length & Format

- 1–2 pages if printed
- **Bullets, not paragraphs**
- No padding — a tight 1-page report beats a sprawling 3-page one every time

---

## Template

Copy this into your Canvas submission and fill it in.

```
═══════════════════════════════════════════════════════════════
                       WEEKLY 4-BOX FORM
═══════════════════════════════════════════════════════════════
TEAM INFORMATION
───────────────────────────────────────────────────────────────
  Team Name     :
  Project Name  :
  Team Members  :
  Week #        :
  Date          : Friday, ____________
  Author        :
═══════════════════════════════════════════════════════════════
  GOALS / KEY TASKS              │  KEY DELIVERABLES
  (next week)                    │  (next week)
───────────────────────────────────────────────────────────────
  •                              │  •
  •                              │  •
  •                              │  •
  •                              │  •
  •                              │  •
═══════════════════════════════════════════════════════════════
  PROGRESS SINCE LAST REPORT     │  RISKS, ISSUES, ACTION ITEMS
  (this week)                    │
───────────────────────────────────────────────────────────────
  •                              │  • Risk:
  •                              │    Impact:    Owner:
  •                              │    Mitigation:
  •                              │
  •                              │  • Risk:
  •                              │    Impact:    Owner:
  •                              │    Mitigation:
═══════════════════════════════════════════════════════════════
```

---

## What Goes in Each Box

### Box 1 — Goals / Key Tasks *(next week)*

What are you committing to do next week? 3–6 bullets. Forward-looking. Each bullet should be specific enough that you can answer "did we do it?" with yes or no a week from now.

| ❌ Bad | ✅ Good |
|---|---|
| "make progress on the front-end" | "Wire the search box to the `/query` endpoint and render the top-3 results with source links" |

### Box 2 — Key Deliverables *(next week)*

What will **exist** by Friday next week? Think artifacts a stakeholder could click on, not activities. Each deliverable should map to a goal in Box 1.

| ❌ Bad | ✅ Good |
|---|---|
| "user testing" | "5 user-test recordings + summary memo with three actionable findings" |

If a deliverable will land in GitHub, paste the branch or PR link. If it's a doc, name it.

### Box 3 — Progress Since Last Report *(this week)*

What actually got done? Use **outcomes, not activities.** If a goal from last week's Box 1 didn't ship, say so explicitly — don't just omit it.

| ❌ Bad | ✅ Good |
|---|---|
| "worked on the retrieval pipeline" | "Replaced default embeddings with `text-embedding-3-large`; retrieval precision on eval set rose from 0.61 to 0.78" |

### Box 4 — Risks, Issues, Action Items

Each item should follow this shape:

- **Description** of the risk or issue  
- **Impact** if not resolved (small / medium / large)  
- **Owner** (a named teammate, not "the team")  
- **Mitigation** or next step with a date

| ❌ Bad | ✅ Good |
|---|---|
| "We might not finish on time" | "Pinecone free tier index size is approaching limit (large impact; Anoushka). Mitigation: prune stale embeddings by Tue; if that doesn't recover headroom, escalate budget request to TA by Wed." |

---

## Rotation

Note the author in the Team Information header. Over 12 weeks, every team member should have authored at least 2–3 reports. Authoring rotation prevents one person from owning all the writing and gives every team member practice translating technical work into stakeholder language.

---

## Grading Rubric

Each weekly 4-Box is worth 10 points. Best 10 of 12 count.

=== "10 — Exemplary"
    All four boxes substantive and specific. Goals are concrete and verifiable. Deliverables are artifacts with working links. Progress uses outcomes (numbers, working features, decisions made), not activities. Risks include impact, named owner, and a dated mitigation. Honest about misses from the prior week. Reads like a real stakeholder report — a busy reader gets the picture in 90 seconds.

=== "9 — Strong"
    All four boxes substantive. Most goals are verifiable; one or two are slightly aspirational. Deliverables map clearly to goals. Progress is outcome-focused. Risks are named with owners but mitigations may lack a date or specific next step. Honest about prior-week misses.

=== "8 — Solid"
    All four boxes filled with reasonable content. Goals are present but a couple are vague ("continue work on X"). Progress is listed but reads as activity rather than outcome ("worked on retrieval"). Risks are real but lack owners or mitigations. Prior-week misses acknowledged in passing.

=== "7 — Adequate"
    All four boxes filled but content is thin or generic. Goals could apply to almost any week. Deliverables are listed without detail or links. Progress reads like a to-do list of what was attempted. Risks are placeholder ("model latency"). No clear authorship or honesty about misses.

=== "6 — Weak"
    Some boxes are sparse or missing. Goals copy-pasted from a previous week with no acknowledgment of carryover. Progress contradicts what's in the GitHub history. Risks box says "none" or is empty.

=== "0 — Not submitted"
    Not handed in by the deadline. Or report contains only the team-information header with all four boxes empty or "TBD."

---

## Calibration Examples

??? example "10 — Exemplary (Cornell Engineering Leadership Training, Week 6)"
    **Team:** Cornell Engineering Leadership Training · **Project:** SBI Voice Coach  
    **Members:** Noefal, Tanush, Anoushka · **Week 6** · **Author:** Anoushka

    **Goals / Key Tasks (next week)**
    - Cut voice→feedback latency from current 4.2s median to ≤2.5s
    - Add tone-shift guardrail: warn user once on aggressive tone, end session on second occurrence
    - Rewrite scenario-setup copy to introduce the SBI framework in ≤3 sentences
    - Replace dashboard placeholder cards with real session-history data
    - Run 3 user tests on the revised setup flow with engineering UGs

    **Key Deliverables (next week)**
    - PR #47: latency optimization (target merge Wed) — [link]
    - PR #48: tone guardrail v2 — [link]
    - Updated `setup.tsx` with new SBI copy — [link to Figma]
    - User-test recordings + 1-page findings memo (Fri)

    **Progress since Last Report**
    - Updated difficulty labels across the interface; verified they map correctly to agent prompt variants (PR #42 merged Tue)
    - Shipped softened-prompt revision for Standard difficulty — eval set "feels too harsh" rate dropped from 38% → 11% on the rerun
    - Implemented off-topic / foul-language detection: warn-once-then-end flow is live (PR #44 merged Thu)
    - **Missed:** dashboard cleanup did not ship — pulled into next week. Reason: blocked on a session-history endpoint that needed schema work.

    **Risks, Issues, Action Items**
    - Voice-model latency baseline of 4.2s too high for coaching feel (large; Tanush). Mitigation: profile pipeline by Tue 3/17; if model is bottleneck, evaluate smaller voice variant by Thu.
    - Tone-shift guardrail could end session abruptly without warning (medium; Noefal). Mitigation: reviewing 20 borderline sessions Mon to tune threshold; PR #48 includes confirmation prompt before terminate.
    - Stakeholder availability for next user-test round unconfirmed (small; Anoushka). Mitigation: emailing recruiter Mon AM with three time options.

    **Why it's a 10:** Specific goals tied to numbers and PRs. Deliverables are linked artifacts. Progress uses outcomes not activities. Misses acknowledged honestly with a reason. Risks have impact, owners, dated mitigations.

??? example "7 — Adequate"
    **Goals:** Continue improving the app · Address feedback from last week · Test more

    **Deliverables:** Updates to the codebase · Bug fixes

    **Progress:** Worked on the voice feature · Made changes to the dashboard · Discussed scenarios with team · Met with Tech Lead

    **Risks:** Latency is a concern.

    **Why it's a 7:** Boxes filled but every bullet is generic. No links. No numbers. No names. Reader cannot tell what shipped or what's at risk.

??? example "6 — Weak"
    Goals copy-pasted from Week 5 with no acknowledgment of carryover. Deliverables: "TBD." Progress: "Made progress on several fronts. Team is collaborating well." Risks: "None at this time."

    **Why it's a 6:** Goals carry over without comment. No deliverables. Progress is filler. "No risks" on a complex project is itself a red flag.
