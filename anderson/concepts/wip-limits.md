---
id: wip-limits
title: "WIP Limits"
type: concept
tags:
- core
- flow
- queueing-theory
- toc
- constraint
links:
- target: wip-constraints
  relation: adapts
  note: Anderson adapted Reinertsen's WIP constraints concept as the core mechanism of the Kanban Method; Reinertsen provided the queueing theory justification
  kb: reinertsen
- target: u-curve-optimization
  relation: related_to
  note: Reinertsen's U-curve (showing optimal utilization below 100%) provides the economic rationale for Anderson's WIP limits
  kb: reinertsen
- target: queueing-theory-applied
  relation: related_to
  note: Reinertsen's queueing theory framework explains why WIP limits improve flow — high utilization causes exponential queue growth
  kb: reinertsen
- target: drum-buffer-rope
  relation: adapts
  note: Anderson's initial Microsoft XIT implementation was directly inspired by TOC's Drum-Buffer-Rope; WIP limits are the knowledge-work adaptation of production pacing
  kb: goldratt
- target: pull-production
  relation: adapts
  note: 'WIP limits implement pull production in knowledge work: work is pulled into a stage only when capacity is available, not pushed by upstream demand'
  kb: tps
- target: just-in-time
  relation: related_to
  note: WIP limits are the JIT principle applied to knowledge work — reducing inventory (WIP) to expose problems and improve flow
  kb: tps
- target: amplify-learning
  relation: related_to
  note: WIP limits amplify learning by shortening feedback cycles — with less work in progress, teams get faster signals about quality and process problems
  kb: poppendiecks
- target: slack-concept
  relation: related_to
  note: "WIP limits create organizational slack: by constraining concurrent work, they preserve capacity for adaptation — connecting Anderson's mechanism to DeMarco's organizational argument"
  kb: demarco
importance: 9
metadata:
  first_appeared: "microsoft-xit-kanban-2004"
  key_writings: &id001
  - kanban-book
  - agile-management-for-software-engineering
  - essential-kanban-condensed
  related_concepts: &id002
  - kanban-method
  - visualize-workflow
  - manage-flow
  - classes-of-service
  - evolutionary-change
  source_tradition: "Reinertsen (queueing theory), Goldratt (TOC)"
  research_status: draft
first_appeared: "microsoft-xit-kanban-2004"
key_writings: *id001
related_concepts: *id002
source_tradition: "Reinertsen (queueing theory), Goldratt (TOC)"
research_status: draft
---

WIP limits — constraints on the maximum number of work items permitted in any workflow stage at one time — are the core operational mechanism of Anderson's [[kanban-method]]. Limiting Work in Progress is what transforms a visualization tool into a pull system; it is the mechanism that forces flow, exposes bottlenecks, and creates the organizational pressure that drives improvement.

## The Mechanism

A WIP limit specifies that a workflow column (e.g., "In Development," "In Review") may hold no more than *n* items simultaneously. When the limit is reached, no new work can enter that column until existing work completes and exits. This creates two effects:

1. **Pull behavior.** Downstream stages pull work only when they have capacity. Work is not pushed into stages regardless of whether they can absorb it.
2. **Bottleneck exposure.** When a stage consistently holds items at its WIP limit while upstream stages sit empty, the limit is revealing a constraint. The system is telling you where the problem is.

The second effect is as important as the first. Anderson frequently emphasized that WIP limits are a diagnostic instrument, not merely a traffic control mechanism. They make dysfunction visible in a way that large batches and full queues obscure.

## Intellectual Sources

### Reinertsen's Queueing Theory

[[don-reinertsen]]'s analysis of product development economics, drawing on M/M/1 queueing models from operations research, provided Anderson with the economic foundation for WIP limits. The key insight: at high utilization rates (close to 100% of capacity), queue length and wait time grow exponentially, not linearly. A system running at 80% utilization has queues roughly four times longer than one running at 50%. The cost in lead time — and therefore in economic value — is enormous.

Reinertsen showed that this was not intuitive to most organizations: people equate idle capacity with waste, but idle capacity in a knowledge work system is what enables fast flow and short queues. WIP limits enforce a utilization ceiling that keeps queues manageable.

### Goldratt's Theory of Constraints

[[eliyahu-goldratt]]'s TOC framework (developed in *The Goal* and applied to projects in *Critical Chain*) provides a complementary logic. TOC argues that every system has one binding constraint and that improving anywhere other than the constraint is local optimization that cannot improve global throughput. WIP limits operationalize this at the workflow level: by forcing focus onto the constraint (the stage that backs up when limited), teams are directed toward the work that matters most for throughput.

Goldratt's distinction between the "throughput world" and the "cost world" is directly relevant: a cost-world mindset treats idle developers as waste and pushes more work into the system; a throughput-world mindset treats long lead times as waste and protects flow by constraining WIP.

## Anderson's Contribution

Anderson's synthesis was to apply these manufacturing and operations research concepts to knowledge work and to package them in a form palatable to software organizations. The early application at [[microsoft]] (2004, see [[microsoft-xit-kanban-2004]]) demonstrated that WIP limits worked for software feature development. The [[corbis-kanban-experiment]] (2007) refined the practice with column-specific limits and the discovery of [[classes-of-service]] as a mechanism for managing different urgency levels within limits.

The key adaptation from manufacturing: in knowledge work, WIP limits must account for the variability of work items (some take days, some take weeks) and the invisible nature of work (unlike physical inventory, software tasks in progress are not self-evidently visible without a [[visualize-workflow]] practice first).

## WIP Limits and Classes of Service

[[classes-of-service]] interacts directly with WIP limits: an Expedite lane typically has a WIP limit of 1 (no more than one expedite item at a time, because expedite items preempt normal flow and create coordination overhead). Standard items have the main column WIP limits. This creates a multi-tiered pull system where urgency is handled structurally rather than through ad hoc escalation.

## Common Misapplications

Anderson documented several failure modes in applying WIP limits:

- **Setting limits too high.** A WIP limit of 20 in a 5-person team does not create useful constraint; it simply formalizes the existing overloaded state.
- **Ignoring the bottleneck signal.** When a column consistently hits its limit, teams sometimes respond by raising the limit rather than addressing the constraint. This defeats the purpose.
- **Limiting WIP without visualization.** WIP limits require a [[visualize-workflow]] practice to be legible; enforcing limits on invisible work is unenforceable.

The [[kanban-book]] addresses each of these through case study analysis, connecting them back to the queueing theory foundations that explain why the failure modes are costly.
