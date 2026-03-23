---
id: adaptive-software-development
title: "Adaptive Software Development"
type: concept
importance: 5
tags:
- methodology
- complex-systems
- highsmith
originator: "jim-highsmith"
concept_type: methodology
research_status: draft
---

Adaptive Software Development (ASD) is a methodology created by [[jim-highsmith]] and described in his book of the same name (2000). It is the lightweight method most explicitly grounded in complex adaptive systems (CAS) theory, drawing on complexity science to argue that software development requires emergence rather than planning. Highsmith brought ASD to [[snowbird-meeting-2001]] as one of the methodology traditions represented.

## Intellectual Foundation: Complex Adaptive Systems

ASD's distinguishing characteristic is its theoretical grounding. Where [[scrum]] draws on industrial process control theory and [[extreme-programming]] draws on software engineering practices, ASD draws on complexity science — specifically the work of Stuart Kauffman, John Holland, and others associated with the Santa Fe Institute.

The CAS argument: complex systems with many interacting components cannot be managed by predicting and controlling their behavior. Instead, they must be allowed to self-organize and adapt. Management of complex systems means setting initial conditions, maintaining edge-of-chaos dynamics (not too ordered to be rigid, not too chaotic to cohere), and creating feedback loops that allow adaptation. Software projects, Highsmith argued, are complex adaptive systems: requirements interact with technology, which interacts with team dynamics, which changes requirements.

This theoretical framing is more sophisticated than is typically recognized in Agile history. [[jim-highsmith]] was engaging with serious complexity science, not just borrowing metaphors.

## The Three-Phase Cycle: Speculate-Collaborate-Learn

ASD replaces the plan-design-build-test-deploy sequence with three phases that recur iteratively:

**Speculate** — not "plan," deliberately. The framing encodes epistemic humility: you are making a bet, not a commitment. Speculate about what to build, how long it will take, what features to include. The speculation should be informed but recognized as uncertain.

**Collaborate** — knowledge creation happens through collaboration among people with different knowledge and perspectives. ASD emphasized collaboration across disciplines (business, technical, customer) as a knowledge-creation mechanism, not just a coordination mechanism.

**Learn** — after each iteration, systematically review what was learned: about the product, about the process, about the domain. Learning is the output of each cycle, not just the product. This connects directly to [[inspect-and-adapt]] and to Deming's PDSA cycle.

## Relationship to Complexity and Emergence

The speculate-collaborate-learn cycle operationalizes the CAS insight. Speculation creates initial conditions. Collaboration enables emergent coordination. Learning implements adaptation. The cycle doesn't optimize toward a predetermined goal; it navigates toward a goal that is itself being discovered.

This makes ASD's theory more radical than most Agile frameworks: it does not just say "respond to change" but explains *why* response to change is structurally necessary in complex systems. [[responding-to-change]] and [[empirical-process-control]] express the same insight, but ASD grounds it in a more explicit theoretical apparatus.

## Legacy

ASD's CAS framing was ahead of its time within the Agile movement but has become increasingly influential in the post-Agile era, as practitioners grapple with why Agile implementations in large organizations produce emergent behaviors their architects did not intend. [[jim-highsmith]] has remained a consistent voice for complexity-informed thinking about organizational agility, extending his work into the Agile 2.0 and business agility discussions.
