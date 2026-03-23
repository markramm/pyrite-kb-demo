---
id: iron-triangle
title: "Iron Triangle"
type: concept
importance: 6
tags:
- project-management
- scope
- constraints
originator: "project-management-tradition"
concept_type: framework
research_status: draft
---

The Iron Triangle — also called the "project management triangle" or "triple constraint" — is the model that defines the fundamental trade-off in project management: scope, time, and cost are interdependent. If you increase scope without changing time or cost, something has to give; if you compress time without changing scope or cost, something has to give. The conventional formulation: "Fast, cheap, good — pick two." (Or equivalently: "Scope, time, cost — pick which two to fix.")

Agile's fundamental project management proposal is an inversion of the conventional Iron Triangle: fix time and cost, and allow scope to vary. This inversion is not merely a tactical preference but the structural mechanism that makes [[responding-to-change]] operationally possible.

## The Conventional Triangle and Its Pathologies

In traditional project management, scope is fixed (by requirements documents, signed contracts, or project charters) and time and cost are allowed to vary as the project encounters reality. This produces characteristic failure modes:

- **Schedule overruns** — scope is fixed, so when delivery is late, time slips
- **Budget overruns** — scope is fixed, so when delivery is more complex than estimated, cost increases
- **Scope cuts at the end** — when both time and budget are exhausted, scope is cut — but at the worst possible time, when the most expensive work has already been done and the least valuable remaining scope is cut from a pile of completed high-cost work

The "iron" in Iron Triangle refers to the immovability of the constraint triangle: you cannot make all three better simultaneously. Any improvement on one dimension costs something on another.

## Agile's Inversion

Agile inverts the triangle by making scope the variable dimension and fixing time (the iteration) and cost (the team). The mechanism:

1. Fix the iteration length (Sprint, timebox): this is not negotiable
2. Fix the team: stable team composition and capacity
3. Vary scope: each Sprint, the team selects from the backlog only what can be completed within the fixed time at the team's actual capacity

This inversion has several consequences. [[velocity]] emerges as the empirical measurement of how much scope fits in a Sprint. [[story-points]] provide the unit for expressing scope in comparable terms. The Product Backlog is prioritized so that the highest-value scope is completed first — when time or budget runs out, the least valuable remaining scope is deferred, not the most valuable recently completed scope.

## The Enabling Condition: [[definition-of-done]]

The Agile Iron Triangle only works if "done" is defined clearly enough to be trusted. If a team can declare scope items "done" without meeting a genuine quality standard, variable scope becomes variable quality — a degenerate case where the triangle appears to balance but actually externalizes cost into [[technical-debt]]. The [[definition-of-done]] is the mechanism that prevents this degeneration: scope varies, but quality is constant.

## Relationship to [[dsdm]] and Timeboxing

[[dsdm]]'s formalization of timeboxing (fixing the duration, varying the scope) is an independent parallel to Agile's Iron Triangle inversion. DSDM's MoSCoW prioritization (Must have, Should have, Could have, Won't have) is a specific technique for managing variable scope within a fixed timebox. Both reflect the same insight: in knowledge work, it is more productive to ask "what is most valuable we can deliver in this time?" than "how long will it take to deliver this scope?"
