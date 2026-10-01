---
title: dev'ing with a genie - a Kent Beck talk
bookmark: https://www.youtube.com/watch?v=F8fBgDCf2Y4
author:
created: 2026-10-01
summary: Kent Beck created Extreme Programming, helped pioneer test-driven development, and was the first signatory of the Agile Manifesto. At Prodacity 2026 he talked about what craft means now that a model i
tags:
  - clippings
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
---
[Kent Beck](Kent%20Beck) created [Extreme Programming](Extreme%20Programming), helped pioneer test-driven development, and was the first signatory of the [Agile Manifesto](Agile%20Manifesto). At Prodacity 2026 he talked about what craft means now that a model is writing much of the code. 

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

## Notes (ai and i)
- In this talk software pioneer *Kent Beck* discusses the evolving nature of **software engineering in the age of AI**. He emphasizes that while AI tools (which he calls "the genie") can generate code quickly, they often produce only "plausible" results that don't actually work, requiring developers to maintain a cynical and rigorous approach to quality (6:47-10:10).
- Uses the term **"the genie"** to refer to AI tools in software development because of the specific, often frustrating nature of the relationship between the human programmer and the AI:
	- **Granting Wishes vs. Delivering Wants:** Like the genie in a fable, the AI grants your exact requests, but the result is often not what you truly wanted or needed
	- **Plausibility vs. Reality:** The AI is exceptionally good at producing "plausible" code -code that looks syntactically correct and convincing at first glance - but it often fails to actually _work_ or perform the task correctly under scrutiny. (**my note on this**: It's clear it now produces largely working code - but how clean and maintainable the code is, is more of an issue)
	- **The Need for Oversight:** Because the AI provides code quickly but unreliably, it requires the human to take an adversarial, cynical view. You cannot assume the code is trustworthy; you must act as a critic to ensure it is not just plausible, but functional

- **Key Takeaways:**
	* **Craft in Augmented Development:** Beck argues that traditional craft—careful naming, decomposition, and structure—still matters, but with different leverage. It is no longer just about the act of programming, but about managing the relationship with AI-generated code (13:06-17:49).
	* **Features vs. Futures:** He introduces a model for software development: developers must alternate between delivering features and investing in "futures" (optionality). Shipping too many features without "resting between the notes" (refactoring/cleaning) leads to a state where future changes become impossible (20:00-26:35).
	* **Iterative vs. One-Shot:** Beck warns against "spec-driven development," which he equates to a new coat for waterfall methodology. He advocates for an iterative approach, emphasizing that true progress is a learning process that "throws off software as a side effect" (34:40-42:15).
	* **Reframing Success:** Drawing on insights from military leadership, he highlights the difference between **effort** (lines of code), **output** (features), **outcome** (user behavior), and **mission** (shared goals). He cautions against Goodhart’s Law: when measures like lines of code become goals, the mission suffers (44:00-48:59).
- **Formal methods** (specifically using the [Lean language](Lean%20language.md)) in the context of his experience with automated development (37:10). He expresses two primary challenges with using formal methods in software engineering:
	- **The "One-Shot" Problem:** Formal methods often feel like a static, "one-shot" process (37:58). If you have a formal specification and prove its properties, but then need to change even a single element of the design, you have to "wind back" your work, which acts as a drag on the iterative change he advocates for.
	- **The Implementation Gap:** There remains an persistent gap between the mathematical model (the formal specification) and the actual running code (38:40). Even after proving that properties hold for a specification, bridging that gap to create a functioning implementation in a language like _C++_ or assembly remains difficult and unresolved (38:55-39:40).
- **One-shot vs Iterative**
	- Kent Beck contrasts these two development paradigms to highlight the risks of modern "spec-driven development" (34:40-35:40):
	- **One-Shot Development:** This approach assumes that if you write a sufficiently detailed specification, the AI (the "genie") can produce the finished, correct software in a single pass (35:28). Beck warns that this is essentially a new coat of paint on **waterfall methodology**—a rigid, linear process that historically failed because it ignores the reality that early decisions need to be informed by later feedback (35:45-36:30).
	- **Iterative Development:** This is the alternative Beck advocates for (35:08). It involves a cycle of deploying software that provides value, observing how users interact with it, and then making informed changes to improve that value (41:28-41:48). He emphasizes that for complex, large-scale systems (like those with millions of users), you cannot simply "re-shoot" the code from scratch; you must build in a way that handles continuity and migration (42:30-43:16).
	- Key Insight: Beck notes that the temptation to use "one-shot" methods often stems from a misunderstanding of how complex software evolves. He argues that true progress is a learning process that treats the code as a side effect, rather than just a finished product defined by a static spec (33:55-34:25).