---
title: dev'ing with a genie - a Kent Beck talk
bookmark: https://www.youtube.com/watch?v=F8fBgDCf2Y4
author:
created: 2026-10-01
summary: Kent Beck created Extreme Programming, helped pioneer test-driven development, and was the first signatory of the Agile Manifesto. At Prodacity 2026 he talked about what craft means now that a model i
tags:
  - ai
  - dev
  - compsci
  - youtube
  - content
rating: 3
category:
  - CompSci
  - Content
  - Tech
collections:
  - blog
aliases:
  - Kent Beck - Software Engineering in the Age of AI
updated: 2026-10-01
---
[Kent Beck](Kent%20Beck) created [Extreme Programming](../../wiki/Computer-Science/Software%20Dev/Extreme%20Programming.md), helped pioneer test-driven development, and was the first signatory of the [Agile Manifesto](Agile%20Manifesto). At Prodacity 2026 he talked about what craft means now that a model is writing much of the code. 

# Kent Beck: Software Engineering in the Age of AI

## In this session: 
- Why Beck calls it the genie, and why plausible code is not working code 
- Features and futures: how every feature you ship burns some of your options for change
- Resting between the notes, and what teams do in the space between features 
- One-shot versus iterative, and why spec-driven development is waterfall wearing a new coat 
- What he found in formal methods with Lean, and the gap he still cannot bridge 
- Effort, output, outcome, mission: a revision Beck worked out during Day 1, and what Goodhart's law does to any measure taken too early 
- Recorded live at Prodacity 2026 in Nashville. Prodacity is Rise8's 3-day training event for GovTech leaders delivering mission-critical software.

![](https://www.youtube.com/watch?v=F8fBgDCf2Y4)

## Notes
- Uses the term **Genie**
	- because of the specific, often frustrating nature of the relationship between the human programmer and the AI
	- and because **you get what you asked for, not what you need (in the long term)**
- **Features vs. Futures** or **"The dark software factory"** where AI generates code so rapidly that it outpaces human understanding and feedback, leading to a brittle codebase that eventually becomes impossible to change (21:35-22:26, 30:46-31:17).
	- To counter this, Beck advocates for a disciplined, **iterative approach** that mimics the "resting between the notes" concept in music. This involves oscillating between two distinct phases:
	*   **The Sprint (Feature Implementation):** Leveraging the "genie" (AI) to quickly build out new functionality or prototypes. During this phase, velocity is prioritized, even if the resulting code is imperfect (22:45-23:12).
	*   **The Pause (Consolidation and Refactoring):** This is the critical step for maintainability. Once a feature is shipped, the human must intentionally step in to:
		*   **Refactor:** Eliminate duplication and improve code readability (24:45-25:02).
		*   **Strengthen Futures:** Proactively improve the design to maintain optionality, ensuring the system remains flexible for future changes rather than becoming a "locked-in" mess (24:35-25:35).
		*   **Verify Learning:** Use the pause as a moment to evaluate what was actually learned during the implementation, rather than just blindly pushing for the next output (32:13-33:15).
- **Formal methods** (specifically using the [Lean language](../../wiki/Computer-Science/Software%20Dev/Languages/Lean%20language.md)) in the context of his experience with automated development (37:10). He expresses two primary challenges with using formal methods in software engineering:
	- **The "One-Shot" Problem:** Formal methods often feel like a static, "one-shot" process (37:58). If you have a formal specification and prove its properties, but then need to change even a single element of the design, you have to "wind back" your work, which acts as a drag on the iterative change he advocates for.
	- **The Implementation Gap:** There remains an persistent gap between the mathematical model (the formal specification) and the actual running code (38:40). Even after proving that properties hold for a specification, bridging that gap to create a functioning implementation in a language like _C++_ or assembly remains difficult and unresolved (38:55-39:40).