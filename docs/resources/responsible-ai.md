# Responsible AI & Data

Building AI tools for real Cornell stakeholders means handling real data, real users, and real institutional trust. Read this page before you touch any client data or start building.

---

## Cornell Data Classification

Cornell classifies data into risk levels. **You must know your project's data risk level before you start building.**

| Risk Level | What it means | Examples |
|---|---|---|
| **Low risk** | Public or non-sensitive data | Published research, public websites, course catalogs |
| **Moderate risk** | Internal university data; not public but not highly sensitive | Internal reports, operational data, staff emails |
| **High risk** | Sensitive personal or regulated data | Student records (FERPA), medical records (HIPAA), financial data |
| **Critical risk** | Highest sensitivity; strict access controls | SSNs, full medical records, security credentials |

!!! danger "Know before you build"
    The Cornell AI Gateway (LiteLLM) and N8N support **moderate risk and below.** If your project involves high-risk data, talk to your Tech Lead immediately — it requires additional review and approval before any data can enter an AI pipeline.

---

## What You Can and Cannot Do With Client Data

### ✅ Allowed

- Use client data within Cornell-approved platforms (AI Gateway, N8N)
- Store client documents in Cornell-managed vector stores
- Build pipelines that retrieve and reference client content to answer questions
- Log AI interactions for debugging, with your Tech Lead's approval

### ❌ Not Allowed

- Paste client data into **any** third-party AI service (ChatGPT, Claude.ai, Copilot chat, etc.) without explicit client and CISO approval
- Commit real credentials, API keys, or passwords to GitHub — ever
- Share client data with other project teams
- Use client data for personal AI experiments outside the project

---

## Academic Integrity: AI Tool Use in This Course

This is an AI engineering course, so we have a deliberate policy on AI tools.

### Writing Code
**AI coding tools are permitted and expected.** Copilot, Cursor, ChatGPT, Claude Code — use them. They are part of professional AI engineering practice. You are responsible for:
- Understanding every line of code you commit
- Being able to explain and defend your architecture choices
- Testing your code, not just accepting AI output

### Writing Individual Assignments
**AI may be used to brainstorm and edit, but not to write.** Your Weekly Reflections (A1), Peer Evaluations (A3), and your portion of the Final Presentation (F3) must represent your own thinking and experience. Specifically:
- ✅ Use AI to help organize, outline, or copy-edit your writing
- ❌ Do not use AI to generate your reflection from a prompt — this defeats the purpose
- ❌ Do not submit AI-generated text as your own without any rewriting

### Code Reviews
**Code reviews must be your own analysis.** Using an LLM to generate review comments without engaging with the code yourself is academic dishonesty.

### Citations
When you use code, prompts, or architecture patterns from a tutorial, blog post, paper, or another repo, link it in a comment or PR description.

---

## Ethical Considerations for Deployed AI

Your tool will be used by real Cornell staff, faculty, or students. Before Demo Day, ask your team:

**Accuracy & reliability**

- What happens when the tool gives a wrong answer? Does the user know?
- Have you tested on edge cases, not just examples that obviously work?
- Is there a human in the loop for consequential decisions?

**Bias & fairness**

- Does your training data or retrieval corpus represent all the users who will use this tool?
- Could your tool produce systematically different quality answers for different user groups?

**Transparency**

- Does the user know they are interacting with AI?
- Does the tool cite its sources so users can verify?
- Does the transition plan (F4) honestly document limitations?

**Privacy**

- Does your tool log user queries? Who can see those logs?
- Is the user data being retained anywhere it shouldn't be?

You don't need to have perfect answers. You need to have asked the questions — and addressed them honestly in your F3 presentation and F4 handoff.

---

## Resources

- [Cornell Data Classification](https://privacy.cornell.edu/data-governance/data-classification)
- [Cornell AI Responsible Use Guidelines](https://ai.cornell.edu/)
- [Cornell Academic Integrity Code](https://theuniversityfaculty.cornell.edu/academic-integrity/)
- [Student Disability Services](https://sds.cornell.edu/)
- [AI Gateway access request (TDX)](https://tdx.cornell.edu/TDClient/39/Portal/Requests/TicketRequests/NewForm?ID=-F3UDBTB1l4_&RequestorType=ServiceOffering)
