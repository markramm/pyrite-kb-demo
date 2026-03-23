---
id: decide-as-late-as-possible
title: Decide as Late as Possible
type: concept
tags:
- lean-software-development
- seven-lean-principles
- decision-making
- optionality
- tps-translation
links:
- target: u-curve-optimization
  relation: influenced_by
  note: Economic framework for optimal decision timing
  kb: reinertsen
- target: pivot
  relation: related_to
  note: Pivoting is deciding at the last responsible moment based on validated learning
  kb: blank
importance: 8
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: set-based concurrent engineering (Allen Ward, Toyota)
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- seven-lean-principles
- last-responsible-moment
- set-based-design
- amplify-learning
- decide-as-late-as-possible
research_status: draft
---

Decide as late as possible is Principle 3 of the [[seven-lean-principles]]. [[mary-poppendieck]] and [[tom-poppendieck]] introduced it in [[lean-software-development-agile-toolkit-2003]] as a translation of Toyota's set-based concurrent engineering — specifically the work of Allen Ward, who studied Toyota's product development process and found that Toyota systematically preserved optionality far longer than Western automakers.

## The TPS Source: Set-Based Concurrent Engineering

[[set-based-design]] is the practice of pursuing multiple design options simultaneously rather than committing early to a single "best" option and iterating from there. Western engineering (point-based design) typically worked by generating a promising concept, evaluating it, modifying it if it failed, and iterating. Toyota instead would maintain several competing design sets in parallel, narrowing them progressively as more information became available, converging to a decision only when the information was sufficient to make a good one.

The advantage of set-based design is not that it is faster in the short run — maintaining multiple options is expensive — but that the final decisions are better because they are made with better information. It also reduces the cost of late-scope changes: when the design space has been kept open, incorporating new requirements late in development is much easier.

## Translation to Software

The Poppendiecks mapped this directly onto software development, where the analogous waste is premature commitment to architectural or requirements decisions. Large upfront design, detailed waterfall specifications, and early technology lock-in all represent decisions made before sufficient information is available. When those decisions turn out to be wrong — as they often do, because the information to make them correctly did not yet exist — the cost of correction is high.

The lean alternative is to identify which decisions are *reversible* and which are *irreversible*, and to defer the irreversible ones until the last responsible moment. This is not procrastination; it is optionality management.

## Last Responsible Moment

The Poppendiecks' operational concept for "decide as late as possible" is the [[last-responsible-moment]]: the point in time at which a decision must be made to avoid foreclosing options. Deciding before the last responsible moment throws away information that will become available. Deciding after it is procrastination — the decision has been delayed past the point where it can be incorporated without penalty.

The distinction is critical because "decide as late as possible" is easily misread as advocacy for delay. The Poppendiecks are explicit that this is a discipline of timing precision, not avoidance. The question is always: *what is the last responsible moment for this specific decision?*

## Connection to Learning

Decide as late as possible is deeply connected to [[amplify-learning]]. The reason to defer decisions is that learning continues up to the point of decision — and the more learning occurs before a decision is made, the better the decision will be. Premature decisions not only lock in potentially wrong answers; they also stop the learning process that might have corrected those answers.

This is why the Poppendiecks treat concurrent options (maintaining multiple design paths) as an investment rather than a waste. The cost of running parallel options is the premium paid for the information that will eventually resolve them.

## Implications for Architecture

In software architecture, this principle argues against "big upfront design" not because planning is bad but because irreversible architectural decisions made with incomplete information tend to be wrong. [[build-integrity-in]] is the complementary principle: integrity is built through ongoing design discipline (refactoring, testing, clear interfaces), not through comprehensive upfront specification. Together, these two principles support an architecture that remains malleable as requirements are learned.

[[donald-reinertsen]] later provided a rigorous economic framework for this insight in *The Principles of Product Development Flow* — the option value of deferring commitment can be quantified using real options theory, giving "decide as late as possible" a precise economic justification that goes beyond intuition.
