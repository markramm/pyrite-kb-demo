---
id: agile-manifesto-twelve-principles
title: "Agile Manifesto Twelve Principles"
type: concept
importance: 9
tags:
- manifesto
- principles
- foundational
originator: "agile-manifesto-signatories"
concept_type: principle
research_status: draft
---

Where the [[agile-manifesto-four-values]] states what Agile teams prefer, the twelve principles explain how those preferences translate into behavior. Published alongside the manifesto at [[snowbird-meeting-2001]], the principles move from customer-facing commitments through team organization to reflection practices. They are more specific than the values, naming concrete patterns — iterations, daily collaboration, face-to-face communication, sustainable pace — while remaining framework-agnostic.

## The Twelve Principles

1. **Customer satisfaction through early and continuous delivery** — "Our highest priority is to satisfy the customer through early and continuous delivery of valuable software." This operationalizes the [[working-software]] value and directly targets waterfall's late-delivery risk.

2. **Welcome changing requirements** — "Welcome changing requirements, even late in development. Agile processes harness change for the customer's competitive advantage." This is perhaps the most radical claim: change is not a failure of planning but a source of value. It connects to [[responding-to-change]] and to [[empirical-process-control]]'s inspection-adaptation loop.

3. **Frequent delivery of working software** — "Deliver working software frequently, from a couple of weeks to a couple of months, with a preference to the shorter timescale." The iteration is the fundamental heartbeat of Agile. [[scrum]]'s Sprint and [[extreme-programming]]'s release planning both instantiate this principle.

4. **Business and developers must work together daily** — "Business people and developers must work together daily throughout the project." The Scrum Product Owner role and XP's on-site customer practice are direct instantiations. Both were reactions to the handoff model where requirements flowed over a wall from "the business" to "IT."

5. **Build projects around motivated individuals** — "Build projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done." This encapsulates the movement's humanistic turn and connects to [[self-organizing-teams]].

6. **Face-to-face communication** — "The most efficient and effective method of conveying information to and within a development team is face-to-face conversation." The most contested principle in the era of distributed and remote work.

7. **Working software as the primary measure of progress** — See [[working-software]]. This principle explicitly repudiates percent-complete metrics and document milestones.

8. **Sustainable pace** — "Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely." See [[sustainable-pace]]. Originally "40-hour week" in [[extreme-programming]] before the Snowbird language was adopted.

9. **Technical excellence and good design** — "Continuous attention to technical excellence and good design enhances agility." This principle is the manifesto's explicit acknowledgment that [[emergent-design]] and [[technical-debt]] management are not optional — technical quality is a precondition for sustained agility.

10. **Simplicity** — "Simplicity — the art of maximizing the amount of work not done — is essential." This connects to lean's waste elimination, to [[kent-beck]]'s "do the simplest thing that could possibly work," and to [[extreme-programming]]'s YAGNI (You Aren't Gonna Need It) principle.

11. **Self-organizing teams** — "The best architectures, requirements, and designs emerge from self-organizing teams." See [[self-organizing-teams]]. The claim that organizational design flows from team autonomy is the architectural corollary of the manifesto's humanism.

12. **Regular reflection and adjustment** — "At regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behavior accordingly." The [[retrospective]] practice is the direct institutionalization of this principle. [[inspect-and-adapt]] is the general pattern it expresses.

## Intellectual Coherence

The twelve principles are not an arbitrary list. They form a coherent system: frequent delivery (1, 3) requires close collaboration (4, 6) from motivated, autonomous teams (5, 11) who maintain technical quality (9, 10) at a sustainable pace (8) and regularly examine whether it is working (12). Welcome change (2) is only viable if working software is always the measure (7) and simplicity keeps the codebase malleable (10). The principles collapse into incoherence if any cluster is selectively ignored — a pattern characteristic of [[dark-agile]] implementations.
