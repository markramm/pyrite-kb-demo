---
id: team-jell
title: "Team Jell"
type: concept
tags:
- teams
- management
- organizational-dynamics
- cohesion
links:
- target: cultural-patterns-of-software-organizations
  relation: related_to
  note: Weinberg's cultural patterns (variable, routine, steering, anticipating, congruent) provide a taxonomy for the organizational cultures that enable or prevent team jell
  kb: weinberg
- target: empower-the-team
  relation: related_to
  note: Team jell (DeMarco/Lister) and empower-the-team (Poppendiecks) describe the same organizational goal from different traditions — Peopleware's sociological observation and lean's management principle
  kb: poppendiecks
importance: 8
metadata:
  first_appeared: "peopleware"
  key_writings: &id001
  - peopleware
  - adrenaline-junkies-and-template-zombies
  related_concepts: &id002
  - peopleware-thesis
  - office-environment-effect
  - flow-and-interruption-cost
  - organizational-learning-disability
  - spanish-theory-of-management
  research_status: draft
first_appeared: "peopleware"
key_writings: *id001
related_concepts: *id002
research_status: draft
---

Team jell is DeMarco and [[timothy-lister|Lister]]'s term for the phenomenon of a team becoming more than the sum of its parts — a qualitative shift in collective performance, identity, and cohesion that cannot be reduced to the capabilities of the individual members. The concept first appears in [[peopleware]] (1987) as a counterpoint to the dominant management model of treating software teams as collections of interchangeable productive units.

## Characteristics of a Jelled Team

DeMarco and [[timothy-lister|Lister]] describe jelled teams by their observable properties rather than by mechanism:

- **Low turnover.** Jelled teams retain their members because people want to stay. High voluntary turnover is a reliable indicator that jell has not occurred or has been broken.
- **Strong group identity.** Members identify with the team as a unit, not just with their employer or their individual role.
- **Shared ownership of outcomes.** Success and failure belong to the team collectively. Members feel personal investment in the quality of group output.
- **Joint enjoyment of work.** Members often report that working in the group is among the most satisfying professional experiences they have had.
- **Sense of eliteness.** Jelled teams often develop a mild conviction that they are doing something special or that they are better than average — not arrogance, but a kind of collective pride that reinforces cohesion.

These characteristics are mutually reinforcing: low turnover enables shared identity, shared identity produces joint ownership, joint ownership creates enjoyment, and enjoyment sustains low turnover.

## Management's Role: Creating Conditions, Not Managing Process

The most important and counterintuitive claim about team jell is about the appropriate management response to it. DeMarco and [[timothy-lister|Lister]] argue that management cannot engineer jell directly — attempts to manufacture team spirit through mandated activities, retreats, or forced team-building typically fail. What management *can* do is create or destroy the conditions under which jell might occur spontaneously.

Conditions that enable jell:
- Stable team membership over time (jell requires time together, and constant reorganization resets the clock)
- Autonomy over how work is done (jelled teams develop their own methods)
- Protected workspace and reduced interruptions (see [[office-environment-effect]] and [[flow-and-interruption-cost]])
- Clear, meaningful goals that the team has some ownership over
- Freedom from defensive management that treats all autonomy as a risk

Conditions that prevent or destroy jell:
- Defensive hiring (refusing to hire anyone better than existing staff)
- Team assassination — breaking up jelled teams because their success is inconvenient, or distributing their members to "spread the talent"
- Pressure and urgency as a permanent management mode (the [[spanish-theory-of-management]] as chronic condition)
- Meaningless work or work that the team cannot take pride in

## Team Assassination

DeMarco and [[timothy-lister|Lister]] name the breaking-up of jelled teams "team assassination" and treat it as one of the most expensive management errors in software. The typical scenario: a team jells over a project, delivers something exceptional, and then management — seeing a group of talented people — distributes them across other projects to maximize coverage. The result is that the jelled team's capability, which was a property of the group and not simply the sum of individual abilities, is destroyed. Each individual carries their own skills to the new assignment; none carries the jell.

The economic argument is that jell takes time to accumulate and cannot be accelerated by management fiat. Destroying a jelled team to optimize short-term resource allocation sacrifices a long-term asset that may take years to rebuild.

## Connection to the Coding War Games

The [[coding-war-games]] data provides indirect support for team jell. The matched-pair analysis showed that performance varied substantially among people from the same organization — and DeMarco and [[timothy-lister|Lister]] observed that organizations with better environmental conditions (the same factors that enable jell) produced better individual performers. While the Coding War Games measured individuals rather than teams, the environmental factors that enable jell and the environmental factors that produce high individual performance are largely the same.

## Later Development

The concept appears in [[adrenaline-junkies-and-template-zombies]] (2008), where team dynamics in crisis-driven and process-driven organizations are analyzed through the lens of patterns. The pathological team patterns in that book are largely recognizable as anti-jell conditions: constant urgency, template compliance as a substitute for judgment, and management by pressure rather than by trust.
