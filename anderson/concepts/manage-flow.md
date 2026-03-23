---
id: manage-flow
title: "Manage Flow"
type: concept
tags:
- core
- flow-economics
- lead-time
- throughput
- lean
links:
- target: flow-control
  relation: adapts
  note: Anderson's manage-flow practice operationalizes Reinertsen's flow-control principles for service-delivery organizations
  kb: reinertsen
- target: cost-of-delay
  relation: related_to
  note: Anderson's flow management aims to minimize lead time, which directly reduces the cost of delay Reinertsen quantifies
  kb: reinertsen
- target: throughput-accounting
  relation: related_to
  note: Anderson's flow management optimizes for throughput — aligning with Goldratt's throughput accounting over traditional cost accounting
  kb: goldratt
- target: common-cause-vs-special-cause-variation
  relation: related_to
  note: Anderson's flow management requires distinguishing systemic (common-cause) variation from special-cause events — the same analytical move Deming's SPC demands
  kb: deming
importance: 7
metadata:
  first_appeared: "agile-management-for-software-engineering"
  key_writings: &id001
  - kanban-book
  - agile-management-for-software-engineering
  - essential-kanban-condensed
  related_concepts: &id002
  - kanban-method
  - wip-limits
  - visualize-workflow
  - classes-of-service
  - fitness-criteria
  source_tradition: "Reinertsen (flow economics), TPS (one-piece flow)"
  research_status: draft
first_appeared: "agile-management-for-software-engineering"
key_writings: *id001
related_concepts: *id002
source_tradition: "Reinertsen (flow economics), TPS (one-piece flow)"
research_status: draft
---

Manage Flow is the third of the six core practices of Anderson's [[kanban-method]]: actively optimizing the movement of work through the system, with lead time, throughput, and smooth flow as the primary performance measures — rather than individual utilization or team velocity.

## What Flow Management Means

In Anderson's formulation, flow management means:

- Monitoring how work items move through the [[visualize-workflow]] board
- Identifying where items stall (blocking, waiting, queue buildup)
- Measuring lead time (time from commitment to delivery) and throughput (items delivered per time period)
- Intervening to restore flow when blockages occur
- Using cumulative flow diagrams (CFDs) and other metrics to understand systemic patterns

The emphasis on flow rather than utilization is a deliberate inversion of the conventional management instinct. Traditional software management measured developer productivity, sprint velocity, or resource utilization. Anderson argued, drawing on [[don-reinertsen]]'s economics, that these measures are proxies at best and counterproductive at worst. An organization running at 100% developer utilization will have terrible lead times because there is no slack capacity to absorb demand variation. Flow management accepts this trade-off explicitly.

## Reinertsen's Flow Economics

[[don-reinertsen]]'s *Principles of Product Development Flow* (2009) provided the theoretical backbone for this practice. Reinertsen applied economic analysis to product development queues, arguing that:

- High utilization → long queues → long lead time → high cost of delay
- The cost of long queues is typically invisible, while the cost of idle capacity is highly visible
- This visibility asymmetry creates systematic management bias toward high utilization and against flow

Anderson translated this into Kanban Method practice: WIP limits enforce a utilization ceiling, and flow management tracks whether the ceiling is achieving its intended effect on lead time and throughput.

## Toyota's One-Piece Flow

[[taiichi-ohno]]'s one-piece flow principle — moving single items through the production process rather than batching — is a direct intellectual source. Ohno showed that large-batch production, despite appearing efficient, hides quality problems, creates large inventories, and extends lead time. One-piece flow makes problems immediately visible and keeps lead time short.

Anderson's adaptation: in knowledge work, "batch size" refers to how much work is grouped in a release, a sprint, or a feature set. The Kanban Method's pull system and [[wip-limits]] create a structural analog to one-piece flow by limiting concurrent work and encouraging smaller, more frequent deliveries.

## Cumulative Flow Diagrams

A key tool in flow management is the cumulative flow diagram (CFD), which plots the count of work items entering and exiting each workflow stage over time. A CFD makes several flow properties directly visible:

- **Throughput** — the slope of the "done" line
- **Lead time** — the horizontal distance between commitment and completion curves
- **WIP** — the vertical distance between arrival and completion curves
- **Bottlenecks** — horizontal plateaus in the diagram (work entering a stage faster than it exits)

Anderson and [[dan-vacanti]] both wrote extensively about CFDs as flow management instruments. Anderson and Carmichael's [[upstream-kanban]] extended this analysis to demand management upstream of the delivery system.

## Flow Efficiency

A related concept developed in the Kanban community: **flow efficiency** is the ratio of active work time to total lead time. Most knowledge work systems have very low flow efficiency — a work item may be "in progress" for 20 days but actively worked on for only 2. The remaining 18 days are queue time: waiting for availability, waiting for review, waiting for approval.

Managing flow means identifying and reducing this queue time, not just maximizing the active work fraction. This is why Anderson positioned Kanban as a systems approach rather than an individual productivity tool: the leverage is in the handoffs and queues, not in making individuals work faster.

## Relationship to Fitness Criteria

[[fitness-criteria]] (from Anderson's later *Fit for Purpose* work with [[dan-vacanti]] and Alexei Zheglov) connects flow management to customer outcomes. A service that delivers with predictable lead time and adequate throughput is "fit for purpose" for customers who need reliable delivery. Flow management provides the operational mechanism for achieving and maintaining that fitness.
