---
id: extreme-programming
title: "Extreme Programming"
type: concept
importance: 9
tags:
- framework
- xp
- technical-practices
originator: "kent-beck"
concept_type: framework
research_status: draft
---

Extreme Programming (XP) is the most technically prescriptive of the Agile methods, created by [[kent-beck]] and first described in [[xp-explained-first-edition]] (1999). Where [[scrum]] is primarily organizational — how to structure the flow of work — XP is primarily technical: how to write code in a way that supports sustained iterative delivery. At [[snowbird-meeting-2001]], Beck represented the XP tradition and brought with him an argument that technical practices and Agile values were inseparable: you cannot sustain rapid iteration without the engineering discipline to support it.

## Values

[[xp-explained-first-edition]] identified four values: communication, simplicity, feedback, and courage. [[xp-explained-second-edition]] (2004, with [[cynthia-andres]]) added a fifth: respect. The values ground the practices — each practice is justified by its contribution to one or more values, rather than being an arbitrary rule.

## Core Practices

XP's practices interlock: removing any one weakens the others.

**[[test-driven-development]]** — Write a failing test before writing code. Forces interface design before implementation, creates a regression suite, and provides immediate feedback. Beck's most enduring contribution to mainstream software practice.

**[[pair-programming]]** — Two developers at one workstation, one driving and one navigating. Continuous code review, knowledge sharing, and defect detection. The most controversial XP practice in enterprise adoption.

**[[continuous-integration]]** — Integrate and test every developer's changes multiple times daily. Eliminates integration hell at the end of long branches. Now a mainstream DevOps practice far beyond the XP context.

**[[refactoring]]** — Continuous restructuring of code to improve its design without changing its behavior. Enabled by the test suite that provides a safety net. The practice that makes [[emergent-design]] operationally feasible.

**[[collective-code-ownership]]** — Any developer can modify any part of the codebase. Prevents knowledge silos and bus-factor risk.

**Planning game** — Customers write story cards (proto-[[user-stories]]); developers estimate; customers prioritize. A precursor to the Product Backlog and Sprint Planning in Scrum.

**Small releases** — Deliver to production frequently. The practice predates the term "continuous delivery" but points toward the same goal.

**Simple design** — "Do the simplest thing that could possibly work." YAGNI: You Aren't Gonna Need It. Prevents speculative complexity.

**On-site customer** — A real customer embedded with the team. The XP predecessor of the Product Owner role.

**Coding standards** — Shared conventions that enable collective ownership.

## XP's Intellectual Contribution

XP established that Agile methodology and technical engineering practices are not separable. The Scrum community's relative silence on technical practices — Scrum does not prescribe how to build software — has been a persistent source of criticism. [[ron-jeffries]] has argued that Scrum's technical agnosticism, combined with organizational pressure, produces teams that commit to sprint goals they cannot sustain because they lack the engineering foundations.

The XP practices have dispersed widely into the broader software engineering mainstream. [[test-driven-development]], [[continuous-integration]], and [[refactoring]] are now standard practice in many contexts with no explicit Agile affiliation. [[pair-programming]] remains contested but is practiced beyond the XP community. XP's technical legacy may exceed its framework adoption in organizational terms.

## The Two Editions

The gap between [[xp-explained-first-edition]] and [[xp-explained-second-edition]] is significant. The second edition dropped several practices (including the "40-hour week" in its original form), restructured the value framework, and adopted a more modest tone about XP's scope. This revision reflects Beck's own evolution and the movement's experience with what worked in diverse organizational contexts.
