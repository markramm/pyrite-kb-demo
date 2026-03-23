---
id: classes-of-service
title: "Classes of Service"
type: concept
tags:
- risk-management
- prioritization
- service-levels
- sla
- expedite
links:
- target: cost-of-delay
  relation: related_to
  note: Anderson's classes of service are risk/urgency categories that map onto different cost-of-delay profiles — expedite items have the steepest delay cost curves
  kb: reinertsen
importance: 8
metadata:
  first_appeared: "corbis-kanban-experiment"
  key_writings: &id001
  - kanban-book
  - essential-kanban-condensed
  - upstream-kanban
  related_concepts: &id002
  - kanban-method
  - wip-limits
  - visualize-workflow
  - manage-flow
  - make-policies-explicit
  - fitness-criteria
  source_tradition: "TOC (constraint-aware prioritization), original"
  research_status: draft
first_appeared: "corbis-kanban-experiment"
key_writings: *id001
related_concepts: *id002
source_tradition: "TOC (constraint-aware prioritization), original"
research_status: draft
---

Classes of Service is Anderson's framework for categorizing work items by their risk profile, urgency, and economic cost of delay — and assigning different workflow policies, WIP limits, and service level commitments to each category. It is one of the most distinctive original contributions of the [[kanban-method]], and it emerged from a specific practical problem at Corbis.

## The Four Standard Classes

Anderson's canonical formulation defines four classes:

1. **Expedite** — items that must be completed as rapidly as possible, preempting normal flow. Typically production incidents, critical customer issues, or regulatory emergencies. Has a separate lane (swim lane) on the board and a WIP limit of 1 (usually) to prevent multiple simultaneous expedites from creating coordination chaos.

2. **Fixed Date** — items with a hard delivery commitment. Missing the date has a known, significant cost (contractual penalty, compliance deadline, major customer demonstration). These items are tracked against their delivery date; as the date approaches, they may be promoted in priority. The cost of delay is defined and binary: miss the date or don't.

3. **Standard** — the majority of work items. No specific deadline or special urgency. Managed by standard WIP limits and first-in-first-out (or similar) ordering within the committed queue. Expected to complete within the team's normal lead time range.

4. **Intangible** — items with low urgency but long-term value: technical debt reduction, infrastructure improvement, learning investments. These items have a non-linear cost of delay — delay itself may not be costly, but indefinite neglect eventually becomes a serious problem. The class acknowledges that these items need to enter the system at some rate, but can yield to other work.

## Origin at Corbis

The classes of service concept emerged organically during the [[corbis-kanban-experiment]]. Drew McLean, a VP at Corbis, asked Anderson's team for an "Expedite" capability — a way to fast-track certain items through the system when business urgency required it. Anderson recognized that this was not a special exception request but an implicit acknowledgment that different work items have different economic profiles and should be managed differently.

This insight — that a single undifferentiated queue treats all work items as economically equivalent when they are not — became the theoretical foundation for classes of service. The Corbis board gained a separate Expedite swim lane with its own WIP limit; the concept then generalized to the four-class framework in [[kanban-book]].

## Cost of Delay as the Theoretical Basis

The underlying economic framework is cost of delay: the economic value lost per unit of time that a work item is not delivered. Different classes of service represent different cost-of-delay profiles:

- **Expedite items** have an extremely high and often nonlinear cost of delay (a production outage is costing money every minute)
- **Fixed date items** have a step-function cost of delay (low until the deadline, catastrophic after)
- **Standard items** have a roughly linear cost of delay (value accumulates progressively)
- **Intangible items** have a low immediate cost but a long-tail risk (technical debt that eventually causes failures)

[[don-reinertsen]]'s cost of delay framework (from *Principles of Product Development Flow*) provides the economic grounding for this differentiation. Anderson applied it to workflow policy design.

## Workflow Policies per Class

Each class of service has associated workflow policies that are made explicit (see [[make-policies-explicit]]):

- **WIP limits** may differ by class (Expedite: 1; others: standard column limits)
- **Aging alerts** may differ (Expedite items trigger escalation quickly; Intangible items may age without alarm)
- **Review cadence** at [[implement-feedback-loops]] meetings may differ
- **Prioritization rules** specify when a Fixed Date item should be pulled ahead of Standard items

These differential policies are the mechanism by which classes of service deliver their value: they are not just labels, but triggers for different handling behavior.

## Classes of Service and Upstream Kanban

Anderson and Carmichael's [[upstream-kanban]] extended the classes of service concept to demand management upstream of the delivery system. Items enter the commitment decision (the Replenishment Meeting) already carrying their class-of-service designation, which shapes how they are prioritized in the pre-commitment queue. This creates end-to-end class awareness: from when a request is first recognized to when it is delivered.

## Connection to Fitness Criteria

[[fitness-criteria]] (from Anderson's later *Fit for Purpose* work) connects directly to classes of service: different customer segments may have different fitness criteria, and classes of service can be designed to match those customer needs. A customer who tolerates 30-day lead times for strategic work but requires same-day response to operational issues needs a class-of-service structure that reflects those different requirements.
