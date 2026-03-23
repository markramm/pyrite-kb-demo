---
id: set-based-design
title: "Set-Based Design"
type: concept
importance: 7
tags:
- lean-software-development
- design
- optionality
- toyota
- tps-translation
first_appeared: "Lean Software Development: An Agile Toolkit (2003)"
tps_source: "set-based concurrent engineering (Allen Ward, Toyota product development)"
key_writings: [lean-software-development-agile-toolkit-2003, implementing-lean-software-development-2006]
related_concepts: [decide-as-late-as-possible, last-responsible-moment, amplify-learning, build-integrity-in]
research_status: draft
---

Set-based design is a product development strategy derived from Toyota's concurrent engineering practice, introduced into lean software development by [[mary-poppendieck]] and [[tom-poppendieck]] in [[lean-software-development-agile-toolkit-2003]] as the manufacturing foundation for the [[decide-as-late-as-possible]] principle.

## Origins: Allen Ward and Toyota Product Development

The concept was documented and named by [[allen-ward]], a researcher at the University of Michigan who studied Toyota's product development process in depth. Ward's research (published with colleagues, and later in *Lean Product and Process Development*, 2007) found that Toyota's approach to concurrent engineering was fundamentally different from the Western norm.

Western product development (point-based design) typically worked by generating a concept, evaluating it, and iterating: propose a design, discover its problems, modify it, repeat. This converges on a solution but discards large amounts of design space early based on incomplete information. When early commitments turn out to be wrong — and they often do — the cost of reversal is high.

Toyota instead pursued *set-based* concurrent engineering: multiple competing design concepts were developed simultaneously, with each set of options kept alive until sufficient information existed to narrow the set intelligently. Teams would not commit to a single design direction until the design space had been explored enough to be confident in the choice.

## The Economic Logic

Set-based design is expensive in the short run: maintaining multiple parallel design paths costs more than pursuing a single path. But it purchases two things of value:

1. **Better decisions.** Decisions made later in the development process are made with more information — test results, customer feedback, technical discoveries, market signals. A decision deferred until that information is available is a better-informed decision.

2. **Lower rework costs.** When a point-based design hits a dead end, the cost of rework is high — often requiring backtracking to a much earlier decision point. Set-based design never fully commits until the decision is robust, so the cost of incorporating new information is lower.

This is essentially an options argument: the cost of maintaining multiple design sets is the premium paid for the option to choose the best path when information becomes available. [[donald-reinertsen]] later formalized this as real options analysis in product development.

## Translation to Software

[[mary-poppendieck]] and [[tom-poppendieck]] applied this to software in two domains:

**Architecture:** Rather than committing early to a single architectural approach, teams can prototype multiple architectures, explore technical feasibility across several options, and converge on an architecture once the key technical uncertainties are resolved. This differs from both "big upfront design" (which commits too early) and from "no design" (which never develops the options fully).

**Requirements:** Rather than specifying requirements exhaustively before development, teams can develop multiple lightweight implementations of competing approaches, learn from them, and converge on requirements as learning accumulates. This is conceptually close to what became story-mapping and hypothesis-driven development in the broader agile community.

## Relationship to Last Responsible Moment

[[last-responsible-moment]] is the timing principle that operationalizes set-based design: the options in a set are maintained until the last responsible moment, then the set is resolved. The discipline is knowing when that moment is — early enough that the decision can be implemented, late enough that it is well-informed.

Together, set-based design and last-responsible-moment decision-making form the Poppendiecks' answer to the waterfall vs. agile debate about upfront planning: neither commit everything upfront nor abandon planning entirely, but structure commitments as options that are exercised at the right time.
