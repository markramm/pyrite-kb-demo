---
id: bounded-rationality-in-systems
title: Bounded Rationality in Systems
type: concept
tags:
- system-dynamics
- decision-making
- cognitive-limits
- policy-resistance
links:
- target: mental-models
  relation: related_to
  note: Meadows's bounded rationality explains why mental models (Senge's second discipline)
    are necessarily incomplete
  kb: senge
- target: psychology-of-management
  relation: related_to
  note: 'Both address cognitive limits: Meadows''s bounded rationality and Deming''s
    psychology component of SoPK'
  kb: deming
- target: common-cause-vs-special-cause-variation
  relation: related_to
  note: Bounded rationality leads managers to misattribute common-cause variation
    to special causes — tampering with stable systems
  kb: deming
- target: orientation
  relation: related_to
  note: Bounded rationality constrains orientation; both Meadows and Boyd emphasize
    that actors operate from incomplete mental models
  kb: boyd
importance: 7
first_appeared: Industrial Dynamics (Forrester, 1961); Beer Game (Sterman, 1989)
source_tradition: system dynamics
key_writings:
- thinking-in-systems-2008
- groping-in-the-dark-1982
related_concepts:
- feedback-loops
- delays-in-systems
- iceberg-model
- system-boundaries
- overshoot-and-collapse
- systems-archetypes
research_status: draft
---

Bounded rationality in systems describes the condition in which actors make individually rational decisions — rational given their information, their incentives, and their cognitive capacities — that collectively produce irrational or damaging system-wide outcomes. The bounded rationality concept originated with Herbert Simon; its application to systems dynamics, particularly through the Beer Game simulation developed at [[mit-system-dynamics-group]], was developed by [[jay-forrester]], [[john-sterman]], and their colleagues, and was central to Meadows's teaching.

The key insight: the problem is not that people are stupid or malicious. The problem is structural. Actors embedded in a system are constrained in what they can see, what they can know, and how fast they can respond. They act on the local information available to them, within the incentive structure they face, using mental models developed from past experience. When the system has long [[delays-in-systems]], complex [[feedback-loops]], and [[system-boundaries]] that exclude the consequences of their actions, individually sensible decisions aggregate into collectively destructive outcomes.

The Beer Game is the canonical demonstration. In the simulation, players managing different nodes of a supply chain (retailer, wholesaler, distributor, factory) each make rational ordering decisions based on their inventory levels and incoming orders. No player is trying to cause problems. Yet the simulation reliably produces wild oscillations in orders and inventories — the "bullwhip effect" — as delays and limited information cause each player to over- and under-order in ways that amplify up the chain. The players did not cause the oscillation; the structure did.

Meadows extended this insight to environmental and social policy. The farmers exhausting a fishery are not irrational: given declining fish populations, the economically rational response for each individual fisher is to catch more while they can, before someone else does. The result is collective overfishing that destroys the fishery everyone depends on. The structure of individual incentives, the absence of enforceable collective-action mechanisms, and the delay between individual exploitation and shared consequences produce the tragedy without any individual acting irrationally.

This has a profound implication for policy. Blaming actors for the bad outcomes of systems is usually wrong: the actors are responding rationally to the information and incentives they face. Changing behavior requires changing the structure — the information flows, the incentive structure, the feedback loops — not just exhorting actors to behave differently. This is why [[leverage-points]] at the level of information flows, rules, and goals outrank appeals to individual virtue.

The [[iceberg-model]] connection: bounded rationality is what makes the structural and mental-model levels of the iceberg invisible to the actors operating at the event level. They see and respond to events; they do not see the structural loops generating those events, because those loops extend outside the boundaries of their information environment and decision-making horizon.

Meadows in [[groping-in-the-dark-1982]] was candid about the implications for modelers as well: even expert analysts are bounded-rational agents, unable to fully verify their models, unable to see all relevant feedbacks, operating with their own paradigm-level assumptions. The [[system-dynamics-meets-the-press]] piece and various reflections from that era show her grappling with what it means to act responsibly under this kind of irreducible uncertainty.
