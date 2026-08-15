# F1 — Working AI Tool

!!! abstract "Submission details"
    **Type:** Team · **Weight:** 10% of final grade  
    **Due:** Monday, Dec 7 (Demo Day)  
    **Format:** Link to GitHub repository  
    **Where:** Canvas → Assignments → Final Deliverables → Working AI Tool

---

## Overview

This is your team's primary artifact: the AI-powered tool you have spent the semester building for your client. It should be **production-ready** (or as close as 12 weeks allows) — working, tested, and deployable without your assistance.

!!! warning "Graders will actually run your code"
    We will clone your repo, follow your README, and attempt to run the tool. If it does not work out of the box, points will be deducted. **Test your own README on a fresh machine before submitting.**

---

## Requirements

- **GitHub repository.** Clean commit history, organized directory structure, no sensitive credentials committed.
- **All core features working.** The features promised to your client in Sprint 1 must be implemented and functional.
- **Automated tests.** At least unit tests covering core AI logic (retrieval, inference, prompt construction). Integration tests preferred.
- **Deployment.** Live URL (Render, Railway, Vercel, HuggingFace Spaces, etc.) or a working Docker image with documented run instructions.
- **README.** Installation, configuration, and basic usage (see [F2](f2-documentation.md) for full documentation requirements).
- **No hardcoded secrets.** API keys and credentials must be in environment variables.

---

## Grading Rubric

This is worth 10 points. The score combines feature completeness, code quality, deployment, and tests — graders consider all of them together rather than averaging sub-scores.

=== "10 — Exemplary"
    All features work reliably on realistic inputs and edge cases. Clone-and-run works in under 30 minutes following only the README. Tests are meaningful and cover the core AI logic plus at least one integration path. Deployment works end-to-end without grader intervention. Code is clean, organized, and free of hardcoded secrets or dead code. Goes beyond the core spec in at least one dimension (latency, UX, robustness, observability).

=== "9 — Strong"
    All core features work; minor bugs but nothing blocks the main use case. Clone-and-run works with one small fix or clarification. Tests cover the main paths meaningfully. Deployment works. Code is well-organized with only minor polish gaps.

=== "8 — Solid"
    Core features work but with a couple of rough edges (one feature handles an edge case poorly, error messages are unhelpful). Tests exist but are limited to happy paths. Deployment works but requires a small undocumented step. Code is functional but uneven in style.

=== "7 — Adequate"
    Most features work but at least one is partially broken or non-functional. Tests are minimal (a handful of unit tests, no integration). Deployment requires troubleshooting or a manual workaround. Code shows signs of last-minute work — duplicated logic, unused branches, scattered TODOs.

=== "6 — Weak"
    Tool runs but core use cases are unreliable. Several features are visibly broken or absent. Tests are token (e.g., `assert 1 == 1`). Deployment fails without team assistance. Code has hardcoded secrets, unhandled exceptions, or major organizational problems.

=== "0 — Not submitted"
    Repo is empty, contains only scaffolding, or doesn't run at all. No working deployment. No README that gets a grader anywhere.

---

!!! tip "Start clean from Day 1"
    Clean commit history is much easier to maintain from the start than to reconstruct at the end. Treat your README as a living document — update it as you build. The grader's 30-minute clock starts when they clone the repo.
