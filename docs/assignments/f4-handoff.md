# F4 — Client Handoff Package

!!! abstract "Submission details"
    **Type:** Team · **Weight:** 10% of final grade  
    **Due:** Monday, Dec 7 (Demo Day)  
    **Format:** Canvas — upload or link to drive/repo accessible to TAs and instructor  
    **Where:** Canvas → Assignments → Final Deliverables → Client Handoff Package

---

## Overview

Your client will need to operate, maintain, and potentially extend your tool after the semester ends — **without you available to answer questions.** The handoff package is everything they need to do that.

Think of it as leaving the project in a state where a competent developer who has never seen it can take over without calling you.

---

## Required Components

1. **Complete codebase.** Final, clean version of all source code. No temporary files, unused branches, or debug code left in.
2. **Environment setup script.** A script (Makefile, bash, or similar) that installs dependencies and configures the environment in one command.
3. **Runbook — operations guide.** Step-by-step instructions for: starting/stopping the service, deploying updates, monitoring for errors, backing up data.
4. **Runbook — troubleshooting guide.** The 5–10 most common failure modes and how to resolve them. Based on problems you **actually encountered** during development.
5. **Credentials and access inventory.** A list of all third-party services used (model APIs, vector DB, hosting, etc.) with instructions for rotating or replacing credentials. **Do NOT include actual keys.**
6. **Transition plan (~1 page).** Summarize: what was built, what was not built (scope cuts), known bugs/limitations, and recommended next steps for a future team.

---

## Suggested Folder Structure

```
/code      — final clean codebase (or link to GitHub tag/release)
/docs      — README, architecture diagram, API documentation, user guide
/ops       — runbooks (operations + troubleshooting)
/handoff   — credentials inventory (no real credentials), transition plan
README.md  — at the root: what is in each folder and how to get started
```

---

## How to Test Your Handoff Package

The best test: **give it to a classmate who was not on your team** and ask them to set up and run your tool using only what is in the package. If they get stuck, you have gaps to fill.

---

## Grading Rubric

This is worth 10 points. The score reflects whether a new operator could take this over without calling the team — not just whether the components exist.

=== "10 — Exemplary"
    All six components present, well-organized, and professional. A developer unfamiliar with the project sets up and runs the tool from the package alone in under 60 minutes. Operations runbook covers normal operation and non-trivial procedures (deploy, rollback, key rotation). Troubleshooting runbook lists 5–10 real failure modes the team actually saw, with the fix the team actually used. Transition plan honestly names what wasn't built, why, and what a follow-on team should do first. Credentials inventory is complete with rotation instructions and zero real keys.

=== "9 — Strong"
    All six components present and useful. Setup works in ≤60 min with one or two small clarifications. Operations runbook covers the main procedures. Troubleshooting has 4–6 real entries. Transition plan is honest and useful. Credentials inventory is complete. Minor polish gaps (e.g., README at the root could be richer; one or two file paths in the runbook are slightly stale).

=== "8 — Solid"
    Five of six components present and useful. One is thin — typically the troubleshooting runbook (1–2 entries, generic) or the transition plan (a paragraph rather than a real handoff). Setup works but takes some trial and error. Operations runbook covers the basics but not edge procedures. Credentials inventory is correct but lacks rotation guidance.

=== "7 — Adequate"
    Four of six components present. Code and basic setup are there; runbooks and transition plan are either missing or one paragraph each. Folder organization is loose. A new operator could probably figure things out but would need to read source code.

=== "6 — Weak"
    Three or fewer components present. Essentially just the codebase plus a README. No runbooks. No real transition plan. No credentials inventory. A new operator at the client site could not run this without contacting the team.

=== "0 — Not submitted"
    No submission in Canvas. Or the linked folder is empty/inaccessible. Or contains only a placeholder document.

---

!!! tip "On the troubleshooting guide"
    This is the component teams most commonly underestimate. The best troubleshooting guides are written **as you hit problems during the semester** — not reconstructed from memory in Week 12. Keep a running doc of every error that took more than 30 minutes to resolve, and what fixed it. That's your troubleshooting guide.
