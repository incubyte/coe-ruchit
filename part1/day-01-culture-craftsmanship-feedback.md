# Part 1 · Day 1 — Incubyte Culture Craftsmanship & Feedback

**Date completed:** 2026-11-12 · **Time spent:** ~4 hours

> Committed to GitHub after the completion date because the submission guidelines changed to Markdown files in a repo. The content was completed on 2026-11-12.

## Success criteria

| Criterion (copied from the planner) | Done? | Evidence (link or section below) |
| --- | --- | --- |
| Understands Incubyte's pod model and values in action | Yes | [Independent Pods](#independent-pods) · [Values in Action](#values-in-action) |
| Understands extreme ownership and collaboration | Yes | [Extreme ownership and collaboration](#extreme-ownership-and-collaboration) · [Exercise 3](#exercise-3-ownership-in-a-remote-pod) |
| Understands craftsmanship discipline in the product role | Yes | [Software craftsmanship](#software-craftsmanship) · [Craftsmanship in the product role](#craftsmanship-in-the-product-role) · [Exercise 4](#exercise-4-craftsmanship-applied-to-a-past-project) |
| Writes a reflection on adjusting to a craft-first environment | Yes | [Reflection](#reflection) |

## Key learnings

### Independent Pods

*Source: Independent Pods, Incubyte Playbook*

- A pod is a small, self-managing team (6 to 8 people) that owns a client initiative with minimal dependency on the client's onshore team.
- The team writes its own Team Charter covering goals, decision-making, accountability, feedback loops and communication.
- The person closest to a problem decides, after asking for advice, and shares the reasoning openly. Big decisions go into ADRs.
- "Work in public" means using team channels by default, not DMs.
- Pods are offer makers, not order takers. Product management is a core pod skill, not something the client supplies.

### Values in Action

*Source: How to Succeed at Incubyte: Values in Action, Incubyte Playbook*

- **Core values:** quality with pragmatism, extreme ownership, proactive collaboration.
- **Aspirational values:** pursuit of mastery; giving, inviting and acting on feedback; creating ecstatic customers.
- For product roles, the playbook names concrete practices: an MVP mindset, BDD, clear Jira tickets, user research and data-driven improvement.

### Software craftsmanship

*Source: Is High Quality Software Worth the Cost?, Martin Fowler*

- Craftsmanship means caring about *how* software is built, not only *what* it does.
- Users can't see internal quality (code structure), so it looks optional. But it decides how fast features can be added. Fowler's example: two identical apps, one with messy code selling for $6 and one with clean code selling for $10. The clean one ships features weekly and wins customers.
- Messy code ("cruft") works like debt. Every new feature pays "interest" on it.
- Low quality is faster only at the very start. Developers feel the slowdown **within a few weeks**.
- Even great teams create cruft. They keep it small with automated tests, refactoring and continuous integration.
- Main lesson: argue for quality with economics, not pride. High internal quality makes future work cheaper, so its real cost is negative.

### Giving feedback

*Source: Industrial Logic, giving feedback*

- The goal is to make people awesome, not to vent.
- Check yourself first: am I calm, am I describing behaviour rather than guessing motives, and is this for them or for me?
- Give it privately, soon, and with permission.
- Structure it with **SBIN**: Situation, Behaviour, Impact, Next.
- Share what you appreciate too, and don't expect instant change.

### Receiving feedback

*Source: Rules for Receiving Feedback, Tim Ottinger, Industrial Logic*

The six rules: listen; no leading questions; don't defend or explain; ask only clarifying questions; don't promise on the spot; thank the person. If you asked for feedback on your work, it's the work being discussed, not you.

### Extreme ownership and collaboration

*Sources: Values in Action and Independent Pods*

- **Extreme ownership, in my words:** I own the outcome, not just my task, including when things go wrong.
- **In a remote team, nobody sees you working,** so ownership has to be visible: quick acknowledgements, updates in team channels, chasing blockers, and following up without reminders.
- **In a pod, the product person often stands in for the client's product owner.** If I wait for direction, the whole pod waits.
- **Collaboration means bringing people in early** (BDD sessions with dev and QA) rather than handing work over at the end.

### Craftsmanship in the product role

*Sources: all of the above, applied to my role*

- **Testable stories:** acceptance criteria and Given / When / Then scenarios agreed with dev and QA before work starts.
- **Thin slices:** small increments we can ship and learn from.
- **Outcomes over output:** every feature has a success metric tied to a user or business goal.
- **Protecting internal quality:** I plan time for tests and refactoring and explain it in terms of cost and speed (Fowler's argument).
- **Recording decisions:** product decisions and their reasons, like engineers' ADRs.
- **For AI features:** eval sets act as the test suite, and every prompt or model change is logged with its reason.

## Exercises

### Exercise 1: Giving feedback with SBIN

**What I did:** wrote feedback for a common product situation using SBIN.

> **Situation:** In Monday's sprint planning,
> **Behaviour:** the login story went into the sprint without acceptance criteria.
> **Impact:** QA couldn't prepare test cases, so testing started two days late.
> **Next:** Can we agree that stories need acceptance criteria before they enter a sprint?

**My reasoning:** the Behaviour line states only what happened. A phrase like "the story was rushed" would be a judgement, which the article warns against. The Next line is a question, not an order, so the other person can say no.

### Exercise 2: Receiving feedback using the six rules

**What I did:** took a likely client situation and compared my instinctive reply with a reply that follows the rules.

| Situation | Instinctive response | Rules applied | Rule used |
| --- | --- | --- | --- |
| A client says the new report screen is "confusing." | "The filters are at the top." | "What were you trying to do? Where did you get stuck?" | Ask only clarifying questions |
| The client asks for a fix by Friday. | "Sure, we'll fix it by Friday." | "Thanks, I'll review this with the team and come back to you tomorrow." | Don't promise on the spot; thank them |

**My reasoning:** the instinctive replies feel helpful, but they explain the problem away and commit the team before we understand it.

### Exercise 3: Ownership in a remote pod

**What I did:** listed everyday situations and compared a task-level response with an ownership response.

| Situation | Task-level response | Ownership response |
| --- | --- | --- |
| A message from a teammate | Reply when I'm free | Acknowledge right away: "Got it, I'll reply by 4 pm." |
| A dependency is stuck | Wait for it | Chase it, and flag the risk with a suggested fix |
| A story is "done" | Close the ticket | Check it against its success metric after release |
| A decision is made in a call | Keep it in my notes | Post it in the team channel with the reason |

**My reasoning:** each ownership response makes my work visible to the team, which matters most when we're remote.

### Exercise 4: Craftsmanship applied to a past project

**What I did:** took a real project from my past work and redesigned how I would run it as a product craftsperson.

**The project:** on a financial analytics platform, I worked on new KPIs for a dashboard prototype. A large QA and maths-verification pass at the end caught several calculation errors, which were fixed late, after the features were built.

| Craft practice | What it would have changed |
| --- | --- |
| Testable stories (Given / When / Then) | Each KPI would have had expected values agreed with dev and QA before building, so errors would surface during development. |
| Thin slices | We would ship and verify one KPI at a time instead of the whole set at once. |
| Outcome metric | We would measure whether users trust and use the KPIs, not just that they were delivered. |
| Decision record | Each formula and the reason for choosing it would be written down, so the maths check has a clear reference. |

**My reasoning:** the errors weren't caused by careless work. They were caused by checking at the end. Moving verification to the start is the same idea as Fowler's cruft argument: the later a problem is found, the more it costs.

## Reflection

What was new for me is that quality here is built in from the start, not checked at the end. On my KPI project, verification was a separate final step, and errors were found after the features were built. Fowler's argument changed how I see this: catching problems early isn't slower, it's cheaper. In future I'll agree test cases and expected values with dev and QA before a story starts. I also want to practise not explaining myself straight away when I receive feedback.

## AI use

- **Tools:** Claude.
- **Used for:** a first draft of notes from the five readings, then reviewing that draft against the planner's success criteria and restructuring it into this template.
- **What I corrected:**
  - Changed my role from "AI Product Manager" to "Product Craftsperson."
  - Removed a claim about a 2024 study that was not in the article I was given and that I could not verify.
  - Cut a long, paraphrased summary of the playbook down to short notes.
  - Removed an AI-feature row from my KPI exercise because that project wasn't an AI feature.
  - Checked the examples and reflection against my own experience.

## Open questions

1. In a pod, who usually owns the Team Charter and the Monthly Readout Report: the product craftsperson or the whole team?
2. Is there a template for recording product decisions, similar to an ADR?

## Changes after review

- None yet.
