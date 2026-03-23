---
id: cultural-patterns-of-software-organizations
title: Cultural Patterns of Software Organizations
type: concept
tags:
- organizations
- maturity
- systems-thinking
- software-management
- culture
links:
- target: the-14-points-for-management
  relation: influenced_by
  note: Weinberg's organizational patterns parallel Deming's 14 Points on management
    culture
  kb: deming
- target: jidoka
  relation: related_to
  note: Both address building quality into the process — jidoka at the machine level,
    Weinberg at the organizational culture level
  kb: tps
importance: 8
first_appeared: qsm-vol1-systems-thinking-1992
source_tradition: ''
key_writings:
- qsm-vol1-systems-thinking-1992
- qsm-vol4-anticipating-change-1997
related_concepts:
- quality-software-management-framework
- general-systems-thinking
- satir-change-model
- congruent-behavior
- moi-model
- programming-as-human-activity
research_status: draft
---

The cultural patterns framework, introduced by [[gerald-weinberg]] in [[qsm-vol1-systems-thinking-1992]], describes five patterns of organizational behavior in software development, from Pattern 0 (complete obliviousness) to Pattern 4 (anticipating change). The patterns characterize how organizations perceive their situation, respond to problems, and manage quality — not as a maturity ladder to be climbed through process compliance, but as a systems-thinking description of how feedback mechanisms and human dynamics actually work.

## The Five Patterns

**Pattern 0: Oblivious.** The organization does not know it has a software process. Projects run by individual heroics and luck. There is no consistent method, no feedback about what works, no organizational memory. Results are highly variable — some projects succeed, some fail, and no one knows why. The organization cannot learn from its experience because it doesn't know what its experience is.

**Pattern 1: Variable.** The organization knows it has a software process, but the process varies wildly by project, team, and individual. Some people are excellent; some are disastrous. There is no organizational standard. Quality depends on who you happen to have on a given project. Weinberg's term "variable" captures this: outcomes vary with people rather than with any organizational capability. This is the pattern of organizations that believe in superprogrammers and heroic rescue projects.

**Pattern 2: Routine.** The organization has established repeatable processes. It can deliver routine projects reliably. But it cannot handle novel problems — anything outside the established routine causes regression toward Pattern 1 behavior. Pattern 2 organizations are comfortable with what they know and brittle in the face of the unfamiliar. Process compliance is high; problem-solving capacity is limited to the domain the process was designed for.

**Pattern 3: Steering.** The organization has feedback mechanisms sophisticated enough to detect and respond to problems as they develop. Managers receive honest information (see [[congruent-behavior]] and the measurement work of [[qsm-vol2-first-order-measurement-1993]]), can interpret it accurately, and can adjust course. The steering metaphor is deliberate: the organization is like a car with functional steering, brakes, and a driver who can see the road — as opposed to Pattern 2, which is like a car that can only drive in a straight line on a flat road.

**Pattern 4: Anticipating.** The organization not only responds to change but anticipates it. It monitors its environment, recognizes early signals of problems and opportunities, and adjusts before crises develop. This requires the feedback mechanisms of Pattern 3 plus organizational capacity for learning and adaptation. Pattern 4 organizations study their own dynamics, run retrospectives that actually change behavior, and build capability for the next class of problems rather than just optimizing for current ones. The [[satir-change-model]] frames Pattern 4 as an organization that has internalized the ability to move through change cycles efficiently.

## Relationship to CMM/CMMI

The Capability Maturity Model, developed at the Software Engineering Institute and influential throughout the 1990s, also describes five levels of software process maturity. The surface similarity is real — both frameworks use five levels to describe progressions from chaos to sophistication — but the underlying logic differs significantly.

CMM defines levels in terms of process artifacts: documented procedures, measurement programs, quantitative management, optimization processes. Progression through CMM levels is achieved by implementing specific process practices. CMM is a process model.

Weinberg's patterns are a systems model. The patterns describe the feedback dynamics and cultural behaviors that characterize organizations at different levels of capability. An organization can have all the process artifacts of a CMM Level 3 organization and still be a Pattern 1 organization in Weinberg's terms, if the processes are not actually followed or if the feedback loops are not actually working. Conversely, a small, informal organization with minimal documented process could be a Pattern 3 or 4 organization if it has genuine feedback mechanisms and congruent communication.

This difference reflects Weinberg's [[general-systems-thinking]] approach: process compliance is a surface indicator; what matters is whether the underlying systems (feedback loops, control mechanisms, human dynamics) are functioning. An organization that improves its CMM rating by writing documents without changing its actual behavior has improved its documentation, not its capability.

## Pattern Transitions and the Satir Change Model

Moving from one pattern to a higher one is not a matter of implementing a checklist. It requires organizational learning — which means going through the [[satir-change-model]]'s change cycle. The introduction of new feedback mechanisms (foreign element) will temporarily disrupt the existing equilibrium (chaos) before the organization integrates the new capability (new status quo at a higher pattern).

Weinberg emphasized that pattern regression is common under stress. A Pattern 3 organization facing a severe crisis will often regress to Pattern 1 behavior — abandoning its feedback mechanisms in favor of heroics and fire-fighting. Building genuine pattern capability means building the organizational resilience to maintain higher-pattern behavior under pressure.

## Practical Use

Weinberg and colleagues at [[aye-conference]] and [[weinberg-and-weinberg]] used pattern diagnosis as an early step in consulting engagements. Identifying the client's current pattern gives a quick read on what kinds of interventions are feasible. A Pattern 0 organization cannot absorb Pattern 3 solutions; it needs to first build basic feedback mechanisms. A Pattern 2 organization needs to develop steering capacity, not documentation. The patterns provide a vocabulary for consulting triage.
