---
id: wip-constraints
title: WIP Constraints
type: concept
tags:
- wip
- flow
- queueing-theory
- kanban
- lean
links:
- target: kanban
  relation: builds_on
  note: Reinertsen's WIP limits for product development are a direct generalization
    of TPS kanban — using card counts to constrain work-in-process and maintain flow
  kb: tps
importance: 9
first_appeared: managing-the-design-factory
key_writings:
- managing-the-design-factory
- principles-of-product-development-flow
related_concepts:
- queueing-theory-applied
- flow-control
- batch-size-reduction
- managing-variability
- cost-of-delay
research_status: draft
---

Work in Process (WIP) constraints — explicit limits on how many items can be simultaneously active in a development system — are the primary operational tool for preventing queue explosion and controlling cycle time. Their mathematical justification derives from [[queueing-theory-applied]], and their economic justification derives from [[cost-of-delay]].

## The Mathematical Foundation

From the M/M/1 queueing model, average queue length grows as ρ/(1-ρ) where ρ is utilization. This function is nonlinear and accelerating: the queue grows slowly at low utilization, then explosively as utilization approaches 100%. A system at 90% utilization has average queue length nine times that of the in-service item. At 95%, it is nineteen times. The relationship means that the last few percentage points of utilization create the most queue — and queue means cycle time, and cycle time means [[cost-of-delay]].

WIP constraints work by bounding the numerator of utilization: if work cannot enter the system beyond a fixed limit, utilization cannot exceed a corresponding ceiling. The system is prevented from operating in the dangerous nonlinear region of the utilization curve.

## Why Utilization Maximization Is Wrong

Standard management intuition says idle resources are waste and utilization should be maximized. This is correct in manufacturing where tasks are homogeneous, variability is low, and the queue dynamics are well understood. In product development, tasks are non-homogeneous, variability is high, and queues are invisible. Maximizing utilization in this context drives the system into the exponential region of the queue-length curve, producing long cycle times that appear as schedule overruns rather than queue costs.

Reinertsen's argument is that some idle capacity is economically optimal — the cost of idle capacity is lower than the [[cost-of-delay]] imposed by the queues that full utilization creates. This is a U-curve trade-off (see [[u-curve-optimization]]) between capacity cost and delay cost.

## Pull Systems and Kanban

WIP constraints implemented as pull systems — where work enters only when capacity is available downstream — are the operational mechanism Reinertsen advocates. Work is pulled by capacity rather than pushed by demand. This prevents queue buildup at bottlenecks and makes the WIP limit self-enforcing.

[[david-anderson]]'s Kanban method for software development drew directly on Reinertsen's queueing analysis to justify WIP limits. Anderson formalized the visualization (Kanban boards with WIP-limited columns) and made the method accessible to practitioners who lacked the mathematical background to derive the limits from first principles. Reinertsen provided the theoretical foundation; Anderson provided the adoption pathway.

## Connection to Flow Control

WIP constraints are the primary tool of [[flow-control]] — active management of the flow state in a development process. Unlike push-based systems that respond to demand, WIP-constrained pull systems respond to capacity, creating a self-regulating mechanism that maintains stable cycle times even as demand varies.

## Queueing Theory Lineage

The application of queue-length limits to control system behavior is standard in telecommunications and operations research. Reinertsen's contribution was importing this framework into product development organizations where it was unknown, attaching economic costs to the resulting queues, and making the prescriptive case for WIP limits on economic rather than cultural grounds.
