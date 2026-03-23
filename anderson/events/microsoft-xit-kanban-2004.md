---
id: microsoft-xit-kanban-2004
title: "Microsoft XIT Kanban Implementation (October 2004)"
type: event
importance: 9
tags:
- kanban-origins
- microsoft
- xit
- pull-system
- first-virtual-kanban
date: 2004-10-01
participants:
- dragos-dumitriu
status: confirmed
---

In October 2004, [[dragos-dumitriu]], manager of Microsoft's XIT (Extended IT) Sustaining Engineering team, requested Anderson's help designing a pull system for managing software support and change requests. The resulting implementation was the first virtual kanban system for knowledge work — a WIP-limited pull system run entirely in software, without physical kanban cards, for an offshore development team in India.

## The problem

The XIT Sustaining Engineering team handled incoming change requests and bug fixes for Microsoft's internal enterprise systems. The team's offshore component in India created a coordination challenge: work was flowing to the offshore team faster than it could be processed, creating a large and poorly managed queue. The team had no reliable mechanism for controlling how much work was in flight simultaneously, and delivery predictability was poor. Dumitriu framed the need explicitly as a "pull system" — a mechanism that would authorize work to enter the development pipeline only when capacity was available.

## Anderson's design

Anderson designed the system drawing on [[eliyahu-goldratt]]'s Drum-Buffer-Rope (DBR) mechanism from Theory of Constraints. The offshore development team was the drum — the constraining resource whose capacity determined the system's pace. A buffer of approved, ready-to-develop work items sat upstream, and a WIP limit (the rope) constrained how many items were in active development simultaneously. When the offshore team completed a work item, it pulled the next item from the buffer, replenishing the buffer from the broader backlog.

The system was implemented on Microsoft Product Studio — Microsoft's internal work management tool — rather than through physical cards or a physical board. This was a crucial innovation: it demonstrated that the kanban concept could be implemented virtually, without the physical infrastructure of Toyota's manufacturing system, and could work for knowledge work where work items are intangible and distributed teams are common.

## Results and significance

The system worked. The offshore team's throughput became more predictable, the queue stabilized, and Dumitriu's team developed visible measures of their work status. Anderson had empirical evidence that a virtual pull system could improve knowledge work delivery — but his theoretical framework for explaining why was still primarily TOC-oriented.

The subsequent conversations with [[don-reinertsen]] in winter 2005 reframed the experiment in queueing theory terms, providing the more rigorous analytical foundation that would support the full Kanban Method. Without the Microsoft experiment, however, there would have been no empirical starting point for that reframing. The [[microsoft-xit-kanban-2004]] event is the origin point of Anderson's intellectual journey toward the Kanban Method — the moment when theory met practice and produced evidence worth explaining.
