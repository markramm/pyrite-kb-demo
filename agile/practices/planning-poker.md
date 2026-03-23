---
id: planning-poker
title: "Planning Poker"
type: practice
importance: 6
tags:
- planning
- estimation
- mike-cohn
- consensus
practice_type: planning
originated_in: "XP / Agile estimation"
status: active
research_status: draft
---

Planning poker is a consensus-based estimation technique in which team members independently select a card from a set (usually a Fibonacci-like sequence: 1, 2, 3, 5, 8, 13, 20, 40, 100) representing their estimate of a work item's relative size, then reveal their cards simultaneously. Divergent estimates trigger discussion; the process repeats until consensus is reached. James Grenning invented the technique around 2002; [[mike-cohn]] popularized it and commercialized the physical card decks, and it became the central technique in [[agile-estimating-and-planning]] (2005).

## Intellectual Contribution

Planning poker's intellectual contribution lies in its management of anchoring bias and dominance effects in group estimation. Conventional estimation in a meeting tends to be anchored to the first number spoken — usually by the most senior or most confident person present. By requiring simultaneous reveal, planning poker prevents anchoring and ensures every team member's estimate is formed independently.

The simultaneous reveal also surfaces disagreement productively. When estimates vary widely (a 3 and a 13), the discussion that follows often reveals a misunderstanding of the story's scope, an unconsidered technical dependency, or a legitimate difference in approach. The estimate divergence is a signal, not just noise.

The use of [[story-points]] — relative rather than absolute units — is a related but distinct choice. Planning poker can be run with hours, points, or t-shirt sizes; its core mechanism (independent estimation, simultaneous reveal) is independent of the unit used. [[mike-cohn]] advocated strongly for story points in combination with planning poker.

## Relationship to Estimation Debates

Planning poker sits at the center of the ongoing Agile debate about estimation. Proponents, including [[mike-cohn]], argue that even imprecise estimates provide valuable information for planning and prioritization. Critics in the "NoEstimates" movement — particularly Vasco Duarte and others — argue that the time spent estimating is waste, and that direct measurements (cycle time, throughput) provide better planning data.

The intellectual tension is real: planning poker produces [[story-points]]-based estimates that feed [[velocity]] calculations, and velocity-based planning has well-documented failure modes (story inflation, velocity gaming). The practice is firmly embedded in the Scrum ecosystem through [[agile-estimating-and-planning]] and the [[succeeding-with-agile]] tradition.

Related practices: [[story-points]], [[sprint-planning]], [[timeboxing]], [[user-stories]].
