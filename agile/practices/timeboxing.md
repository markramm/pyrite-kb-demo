---
id: timeboxing
title: "Timeboxing"
type: practice
importance: 7
tags:
- planning
- scrum
- dsdm
- fixed-time
practice_type: planning
originated_in: "DSDM / Scrum"
status: active
research_status: draft
---

Timeboxing is the practice of fixing a duration for an activity and completing the best possible work within that duration, rather than fixing scope and allowing duration to vary. In software development, the sprint is the canonical timebox: its length is fixed (one to four weeks), and scope is variable — the team delivers whatever can be completed to the [[definition-of-done]] within the period. This inverts the traditional project management assumption, which fixes scope (requirements) and estimates time.

Timeboxing was a foundational principle of [[dsdm]] before Scrum popularized it. [[scrum]] made the sprint the organizing structure of software development, and the [[scrum-guide]] defines all Scrum events as timeboxed: the Sprint itself, sprint planning, daily standup, sprint review, and retrospective each have maximum durations.

## Intellectual Contribution

Timeboxing's intellectual contribution is the reframing of the [[iron-triangle]] (scope, time, cost). Traditional project management treats scope as fixed and negotiates time and cost. Timeboxing fixes time (and, by implication, cost) and negotiates scope. The result is a fundamental shift in what kind of problem delivery becomes: instead of "when will we finish X?", the question becomes "what is the most valuable thing we can deliver in the next sprint?"

This reframing makes the [[responding-to-change]] principle operational. When scope is fixed, a change request is a disruption to the plan — it requires re-estimation, re-scheduling, and often re-negotiation of the contract. When time is fixed and scope is variable, new information simply changes what is built next sprint; it does not threaten the delivery timeline.

Timeboxing also serves as a forcing function for [[inspect-and-adapt]]. A fixed period with a fixed endpoint creates a natural rhythm of integration, review, and adjustment. Without the timebox, teams can perpetually defer feedback by extending the current phase.

## Connection to Other Practices

Every major Scrum event is a timebox: [[sprint-planning]], [[daily-standup]], [[sprint-review]], and [[retrospective]] all have maximum durations. The timebox disciplines meetings as well as development cycles, operationalizing the [[agile-manifesto-twelve-principles]] preference for minimal bureaucracy.

[[dsdm]] made timeboxing central to its methodology before the Agile Manifesto, and the [[snowbird-meeting-2001]] drew participants (notably [[arie-van-bennekum]]) who carried this tradition. Timeboxing predates Agile in project management literature (James Martin discussed it in RAD methodologies in the early 1990s).

Related practices: [[sprint-planning]], [[sprint-review]], [[retrospective]], [[daily-standup]], [[story-points]].
