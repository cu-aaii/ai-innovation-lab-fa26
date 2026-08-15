# Tools & Platforms

This page covers the tools you will use in this course. Your Tech Lead will provision access to most of these during Weeks 1–2. If you're waiting on access, contact your TA.

---

## Required Tools

### GitHub
**What it is:** Version control and code collaboration  
**Why we use it:** All project code lives here. Your final deliverable (F1) is a GitHub repo.  
**Access:** Share your GitHub username with your TA in Week 1. You will be added to the team repo under the [`cu-aaii`](https://github.com/cu-aaii) org.  
**Key rule:** No hardcoded secrets, ever. No sensitive credentials committed, ever.

---

### Microsoft Teams
**What it is:** Team communication platform  
**Why we use it:** Day-to-day communication with your team, Tech Lead, TA, and stakeholders  
**Access:** Cornell NetID login at [teams.microsoft.com](https://teams.microsoft.com)  
**Key rule:** Acknowledge messages within 24 hours. Batch your questions — don't send 7 separate Teams messages in a row.

---

### Zoom
**What it is:** Video conferencing  
**Why we use it:** All client sprint meetings are held over Zoom  
**Access:** [cornell.zoom.us](https://cornell.zoom.us) — log in with your Cornell NetID  

---

### Canvas
**What it is:** Cornell's LMS  
**Why we use it:** All assignment submissions, grades, announcements, and the official syllabus  
**Access:** [canvas.cornell.edu](https://canvas.cornell.edu)  
**Key rule:** Check Canvas at least once a week. Announcements are posted here, not just Teams.

---

## AI Development Tools

### Cornell AI Gateway (LiteLLM)
**What it is:** Secure, Cornell-hosted access to frontier AI models (GPT-4o, Claude 3.x, etc.)  
**Why we use it:** Builds AI features without sending data to external APIs. Required for anything touching client data.  
**Access:** Pilot phase — provisioned by your Tech Lead upon request  
**Data risk:** Supports moderate-risk data and below  
**Portal:** [api.ai.it.cornell.edu](https://api.ai.it.cornell.edu)

---

### N8N / AI Agent Studio
**What it is:** Visual agentic workflow builder  
**Why we use it:** Build and manage AI agents and multi-step workflows without writing all the orchestration code from scratch  
**Access:** Pilot phase — your Tech Lead will set up your workspace  
**Data risk:** Supports moderate-risk data and below  
**Portal:** [n8n-dev.lcmain.aaii.cucloud.net](https://n8n-dev.lcmain.aaii.cucloud.net)

---

### Microsoft 365 Copilot Chat
**What it is:** General-purpose GenAI (GPT/DALL-E) via Microsoft  
**Why we use it:** Day-to-day productivity tasks, drafting, coding assistance  
**Access:** Available to all Cornell faculty, staff, and students 18+; free  
**Data risk:** Low-risk only — uses Microsoft's public search, so privacy is limited. **Do not use with client data.**

---

### Anthropic Claude / Claude Code
**What it is:** Anthropic's suite — Claude.ai (chat), Claude Code (coding), Claude Cowork (desktop automation)  
**Why we use it:** Coding assistance and AI-assisted development workflows  
**Access:** Under review — Cornell is working with Anthropic on a higher-ed compliant offering  
**Data risk:** TBD — check with your Tech Lead before using with any client data

---

## Cornell's AI Tool Framework

Cornell uses a **Core-Common-Unique** framework to manage AI tools:

| Layer | What it means | Examples |
|---|---|---|
| **Core** | Institution-wide, managed centrally | Copilot Chat, Gemini, AI Gateway |
| **Common** | Centrally hosted, locally adapted | MCP servers, enterprise integrations |
| **Unique** | Specialized, domain-specific | Harvey AI (legal), medical imaging AI, unit-developed tools |

When choosing a tool for your project, always start with Core tools. Escalate to your Tech Lead if a Core tool can't meet your needs.

---

## Data Risk Reminder

!!! danger "Client data stays in approved systems"
    Do not paste stakeholder data, internal documents, or non-public credentials into any third-party AI service. Use only model providers approved by the course or your client. When in doubt, ask your Tech Lead before pasting anything into an AI tool.

    See [Responsible AI & Data →](responsible-ai.md) for the full policy.
