# A1 — Weekly Reflection

!!! abstract "Submission details"
    **Type:** Individual · **Weight:** 10% of final grade  
    **Due:** Every Friday by 5:00 PM ET (best 10 of 12 count)  
    **Format:** Text entry on Canvas (no file upload)  
    **Where:** Canvas → Assignments → Weekly Reflection (Week #)

---

## Overview

Each week you write a short reflection connecting your experience that week: code you wrote, meetings you attended, feedback you received. Reflections are **not summaries**. They are evidence that you are thinking about your own work, your team dynamics, and the broader context of building AI tools for real clients.

Reflections are due every Friday regardless of which weekday your sprint is scheduled.

**Best 10 of 12 count.** You can skip 2 with no effect on your final grade — or submit every week and drop the 2 lowest.

---

## Length & Format

- **250–400 words**
- No specific format required — write in first person
- Should reflect on the **previous week's** work

---

## Suggested Weekly Prompts

These are suggestions only. You may write about anything relevant and interesting from your week.

| Week | Suggested prompt |
|---|---|
| 1 | What excites you most about working on a real AI project this semester? What is your biggest question or worry? |
| 2 | What did you learn from your first team meeting and client kickoff? What is still unclear about the project? |
| 3 | What surprised you during sprint planning? How did your team decide what to build first? |
| 4 | What was the hardest part of Sprint 1 so far? What is your specific contribution to the sprint? |
| 5 | What did you learn from giving or receiving a code review this week? What would you do differently? |
| 6 | You are now halfway through the semester. What is one thing you are proud of, and one thing you want to improve? |
| 7 | How is your team handling technical decisions (e.g., which model to use, how to structure the pipeline)? What is your role in those conversations? |
| 8 | Describe a moment this week where you got stuck. How did you resolve it — or how are you still trying to? |
| 9 | What feedback have you received from your Tech Lead or TA that changed how you approached something? |
| 10 | You are entering the final stretch. What is the most important thing left to do, and what is your plan? |
| 11 | How is your team preparing for the final presentation and client handoff? What is your specific role? |
| 12 | What did you build this semester? What are you most proud of, and what would you do differently if you had another month? |

---

## Grading Rubric

Each reflection is worth 10 points.

=== "10 — Exemplary"
    Specific, thoughtful, and honest. Includes a concrete, well-chosen example (code, conversation, decision, failure) and reflects on it with genuine insight. Connects experience to course learning in a way that goes beyond the obvious. 250–400 words.

=== "9 — Strong"
    Specific and thoughtful, with a concrete example and a clear connection to learning. Solid reflection but lacks the extra depth, surprise, or self-awareness of an exemplary entry. 250–400 words.

=== "8 — Solid"
    Includes a specific example and connects to learning, but stays on the surface — observations are reasonable but not particularly probing. Meets length requirement.

=== "7 — Adequate"
    General observations with limited specificity. Meets length requirement but lacks depth.

=== "6 — Weak"
    Vague, summary-like, or off-target. Little real reflection, thin content. May be under length.

=== "0 — Not submitted"
    Not handed in. Or a submission that is clearly not a reflection (e.g., a summary of what AI is with no personal experience).

---

## Examples

The same prompt — *"Reflect on a moment this week when you used AI for your work"* — written at each quality tier.

??? example "10 — Exemplary"
    This week I asked Claude to help refactor a Python script that scans TDX tickets for FAQ candidates. My first prompt was "make this cleaner" and I got back a version that was technically tidier but had silently dropped the date-filtering logic — which was the whole point. I didn't catch it until I ran the script against last month's tickets and got 4x the expected matches.

    What I learned isn't really about Python. It's that "cleaner" is a meaningless instruction when I haven't articulated what the code is for. The model optimized for legibility because that's what I asked for; it had no way to know date-filtering was load-bearing. The next prompt I wrote started with "this script's job is X, the date filter is critical because Y, now suggest refactors that preserve that behavior" — and the output was usable.

    This connects to what we discussed about specification being the actual skill. I keep treating prompts like requests to a person who shares my context. They aren't. The model has whatever context I put in the prompt, full stop. The bug wasn't in the code; it was in my framing.

    **Why it's a 10:** Specific moment, real failure, honest about own contribution to the problem, connects to a course concept in a non-obvious way.

??? example "9 — Strong"
    I had Claude help draft a Jira ticket from a Teams thread this week. It pulled the right action items but assigned them all to me, even though two were clearly for someone else. I had to manually reassign before submitting.

    What I took from this: the model defaults to whoever's perspective it's seeing the conversation from. That's obvious in hindsight but I hadn't thought about it. Now I add a sentence in my prompt clarifying who's responsible for what before asking it to draft the ticket.

    This relates to our discussion of context windows — the model isn't reading minds, it's reading the text I give it, and missing context shows up as confident-but-wrong defaults.

    **Why it's a 9, not 10:** Specific, honest, connects to learning. Slightly less depth — the insight is real but more "tip I learned" than "shift in how I think."

??? example "8 — Solid"
    This week I used AI to help write a summary of the AI Hub's intake process. I gave it rough notes and it produced a clean draft. I had to edit it for tone — it was too formal — but the structure was good and saved me time.

    I think the lesson is that AI is good at structure but I still need to handle voice. That fits with what we read about AI being a draft tool, not a finished-product tool.

    **Why it's an 8:** Specific example, connects to course material, but the reflection is surface-level. No real tension or surprise.

??? example "7 — Adequate"
    I used AI a few times this week, mostly for drafting emails and summarizing documents. It was helpful overall. Sometimes the output needed editing but it was usually a decent starting point. I think AI is most useful when you have a clear idea of what you want before you ask.

    **Why it's a 7:** Hits the prompt, mentions usage, draws a generic conclusion. No specific moment, no concrete example, nothing personal.

??? example "6 — Weak"
    AI tools are useful but you have to check the output. I used Claude this week and it worked fine. The main thing I learned is that you can't trust everything it says. Prompting matters too.

    **Why it's a 6:** Generic AI commentary, not a reflection on the writer's own week. Could have been written without doing the work.
