# F2 — Technical Documentation & User Guide

!!! abstract "Submission details"
    **Type:** Team · **Weight:** 10% of final grade  
    **Due:** Monday, Dec 7 (Demo Day)  
    **Format:** Canvas upload or link  
    **Where:** Canvas → Assignments → Final Deliverables → Technical Documentation & User Guide

---

## Overview

Great AI tools fail in production because no one knows how to run them. Your documentation package must:

1. Enable a **new developer** to set up and run your tool within one hour
2. Enable a **non-technical client stakeholder** to understand what it does and how to use it

---

## Required Components

- **README.md** — Project purpose, architecture overview, tech stack, quick-start instructions
- **Developer setup guide** — Step-by-step environment setup (OS requirements, dependencies, env variables, database seeding if applicable)
- **API documentation** — Every endpoint with request/response schema, authentication, error codes (OpenAPI/Swagger or equivalent preferred)
- **Architecture diagram** — Visual of how data flows through the system (retrieval pipeline, model calls, storage)
- **User guide** — How a non-developer uses the tool, with screenshots or annotated UI walkthrough
- **Deployment guide** — How to deploy to production from scratch

---

## Tips

- Write documentation **as you go** — do not leave it all for Week 12
- Have a teammate who did not write a feature try to set it up using only your docs
- Screenshots and code snippets are better than paragraphs of description
- Keep the user guide jargon-free — write for your actual client, not for your TA

---

## Grading Rubric

This is worth 10 points. The score reflects all six required components together — not an average — with weight given to whether a new developer (and a non-technical user) could actually use the tool from the docs alone.

=== "10 — Exemplary"
    All six components present and high quality. Architecture diagram is accurate and named-component-by-named-component matches the code. README enables a new developer to deploy in ≤60 min with no surprises. User guide is jargon-free, includes annotated screenshots, and a non-technical reader can follow it. API docs cover every endpoint with examples and error cases. Includes a troubleshooting section based on real issues the team hit.

=== "9 — Strong"
    All six components present. README and setup work cleanly. User guide is clear with screenshots. Architecture diagram is accurate but slightly schematic. API docs cover all endpoints but a couple of error cases are skipped. Troubleshooting section is present but short.

=== "8 — Solid"
    Five of six components present and useful; one is thin (e.g., user guide is text-only with no screenshots, or troubleshooting is missing). Setup instructions are correct but assume some context a new developer might not have. Architecture diagram is high-level but not wrong.

=== "7 — Adequate"
    Four of six components present. Either API docs or user guide is missing; troubleshooting is absent. README gets a developer most of the way but requires trial-and-error or reading code to finish setup. Architecture diagram is missing or is a generic stock image.

=== "6 — Weak"
    Three or fewer components present. README is sparse — a few sentences and a `pip install` line. User guide is absent or a screenshot with no labels. Architecture diagram missing. A new developer cannot set up the tool from the docs alone.

=== "0 — Not submitted"
    No documentation submitted. Or documentation link is broken/private. Or documentation is empty placeholder text.
