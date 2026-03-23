---
id: empirical-process-control
title: "Empirical Process Control"
type: concept
importance: 8
tags:
- scrum
- foundations
- process-theory
originator: "ken-schwaber"
concept_type: framework
research_status: draft
---

Empirical process control is the theoretical foundation of [[scrum]]. [[ken-schwaber]] drew on industrial process control theory — specifically the distinction between defined processes and empirical processes — to argue that software development cannot be managed like manufacturing. The argument provides Scrum with its philosophical grounding and distinguishes it from plan-driven methodologies at a level deeper than practice differences.

## Defined vs. Empirical Process Control

**Defined process control** assumes that a process can be fully specified in advance. Given the same inputs and the same process steps, you get the same outputs. Assembly lines exemplify defined processes: variance is a defect, and the goal is eliminating variance. Traditional waterfall project management imported this model into software: specify requirements, follow the defined phases, deliver the specified output.

**Empirical process control** applies to processes that are too complex or too variable to be fully specified. Instead of defining the process upfront, you rely on frequent inspection of actual outputs and adaptation of the process based on what you observe. The pharmaceutical industry's FDA approval process is Schwaber's canonical example: you cannot predict drug interactions from theory alone, so you run trials, inspect results, and adapt.

Schwaber's insight was that software development resembles the empirical case, not the defined case. Requirements are discovered, not specified. Technology introduces unexpected constraints. Team performance varies. Attempting to manage software through defined process control produces the pathologies that characterized 1990s enterprise software: late delivery, scope cuts, and projects that delivered what was specified rather than what was needed.

## The Three Pillars

The [[scrum-guide]] formalizes empirical process control through three pillars:

**Transparency** — the process and its outputs must be visible to those responsible for the outcome. Transparency is precondition for inspection: you cannot inspect what you cannot see. Scrum's artifacts — Product Backlog, Sprint Backlog, Increment — are transparency mechanisms.

**Inspection** — Scrum events are inspection points: the [[sprint-review]] inspects the Increment against the Sprint Goal, the [[retrospective]] inspects the team's own process. Inspection must be frequent enough to detect problems before they compound.

**Adaptation** — when inspection reveals that the process is deviating from acceptable limits, the process or the work must be adjusted. The Product Owner adapts the backlog; the team adapts its practices in the retrospective. Adaptation is what distinguishes empirical control from mere observation.

## The [[inspect-and-adapt]] Loop

Empirical process control expresses itself as a feedback loop: inspect what actually happened, adapt the plan based on what you learned, execute again. This loop runs at multiple timescales in Scrum: daily (Daily Scrum), each Sprint (Sprint Review and Retrospective), and across Sprints (backlog refinement). The pattern is structurally equivalent to Deming's PDCA cycle and to [[kent-beck]]'s test-driven development loop, which are themselves instances of the same empirical control logic.

## Significance for the Movement

Schwaber's use of process control theory gave [[scrum]] — and by extension the broader Agile movement — a principled argument against waterfall that was independent of values or preferences. The argument is not that waterfall is wrong because it is bureaucratic or dehumanizing, but that it is wrong for software because it applies the wrong model of process control. This theoretical grounding contributed significantly to Scrum's spread in organizations that were skeptical of the softer claims about teams and values.
