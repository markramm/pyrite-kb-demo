---
id: kanban-method
title: "Kanban Method"
type: concept
tags:
- core
- change-management
- evolutionary
- knowledge-work
- six-practices
links:
- target: buffer-management
  relation: related_to
  note: Kanban's WIP limits and classes of service function as buffer management mechanisms adapted from TOC for knowledge work
  kb: goldratt
- target: system-of-profound-knowledge
  relation: related_to
  note: "The Kanban Method draws on all four components of Deming's System of Profound Knowledge: appreciation for a system, knowledge about variation, theory of knowledge, and psychology"
  kb: deming
- target: appreciation-for-a-system
  relation: related_to
  note: The Kanban Method treats the workflow as a system — WIP limits, feedback loops, and visualization are mechanisms for developing systemic understanding
  kb: deming
- target: kanban
  relation: adapts
  note: Anderson adapted Toyota's kanban production signaling system into a change management method for knowledge work — same name, fundamentally different application
  kb: tps
- target: eliminate-waste
  relation: related_to
  note: WIP limits reduce work-in-progress inventory — a direct application of the Poppendiecks' lean waste elimination principle to knowledge work queues
  kb: poppendiecks
- target: seven-wastes-of-software
  relation: related_to
  note: "Kanban's visualization and WIP limits make several of the seven wastes visible: partially done work (WIP), task switching, waiting, and handoffs"
  kb: poppendiecks
importance: 10
metadata:
  first_appeared: "corbis-kanban-experiment"
  key_writings: &id001
  - kanban-book
  - agile-management-for-software-engineering
  - essential-kanban-condensed
  - discovering-kanban
  - kanban-alternative-path-to-agility
  related_concepts: &id002
  - wip-limits
  - visualize-workflow
  - manage-flow
  - make-policies-explicit
  - implement-feedback-loops
  - improve-collaboratively
  - evolutionary-change
  - classes-of-service
  - statik
  source_tradition: "original synthesis (TPS, TOC, Reinertsen, Deming)"
  research_status: draft
first_appeared: "corbis-kanban-experiment"
key_writings: *id001
related_concepts: *id002
source_tradition: "original synthesis (TPS, TOC, Reinertsen, Deming)"
research_status: draft
---

The Kanban Method is David Anderson's formulation of an evolutionary change management approach for knowledge work services. It is not a project management methodology and not a repackaging of Toyota's kanban production scheduling system — it is a specific framework that uses a kanban board and WIP limits as mechanisms to surface and resolve organizational problems incrementally, without requiring wholesale process replacement.

## What the Method Is and Is Not

The name creates persistent confusion. [[taiichi-ohno]]'s kanban system at Toyota was a physical signal card used to regulate inventory and production pull in a manufacturing context. Anderson's Kanban Method appropriates the pull-system logic and visual card mechanics but applies them to knowledge work — software development, IT operations, creative services — where work is non-repeatable, invisible, and deeply variable. The source inspiration is acknowledged; the method is original.

The Kanban Method explicitly does **not** prescribe:
- Specific roles (no "Kanban Master," no required team structures)
- Ceremonies or meeting cadences (these emerge from the [[implement-feedback-loops]] practice but are not mandated)
- Iteration lengths or sprints
- Story formats or estimation techniques

This distinguishes it sharply from Scrum, which Anderson positioned as the alternative. Scrum requires a specific role set, ceremony calendar, and iteration rhythm before it can be "done." The Kanban Method says: start with what you do now.

## The Three Core Principles

The mature formulation (from [[kanban-book]] and subsequent teaching) rests on three foundational principles:

1. **Start with what you do now.** Do not disrupt existing processes, roles, or responsibilities. Overlay the method on the current system.
2. **Agree to pursue incremental, evolutionary change.** The organization commits to gradual improvement rather than revolutionary transformation.
3. **Respect the current process, roles, responsibilities, and titles.** Existing arrangements represent accumulated organizational knowledge and political settlement; they should be evolved, not discarded.

These principles make adoption politically low-risk, which Anderson identified as critical for consulting engagements. Scrum's disruptive model required organizational buy-in that was often unavailable. The evolutionary approach built on what existed.

## The Six Core Practices

The method's operational content is expressed in six practices, developed cumulatively through Anderson's consulting and writing:

1. **[[visualize-workflow]]** — make work and its states visible on a board
2. **[[wip-limits]]** — constrain concurrent work to improve flow and expose bottlenecks
3. **[[manage-flow]]** — optimize for smooth flow of work through the system
4. **[[make-policies-explicit]]** — document and share the rules governing work
5. **[[implement-feedback-loops]]** — establish regular cadences for review and adaptation
6. **[[improve-collaboratively]]** — use models and the scientific method to evolve the system

The practices build on each other. Visualization makes WIP visible; WIP limits make flow manageable; explicit policies make the system legible to everyone; feedback loops create improvement opportunities; collaborative improvement closes the cycle.

## Intellectual Sources

Anderson is explicit about his sources. The method draws from:

- **[[taiichi-ohno]]** and the Toyota Production System: pull systems, visual management, kanban cards as scheduling signals
- **[[don-reinertsen]]**'s product development flow economics and queueing theory: the economic cost of WIP, [[wip-limits]] as queue management, flow efficiency
- **[[eliyahu-goldratt]]**'s Theory of Constraints: focus on the system constraint, throughput accounting, the cost of local optimization
- **[[w-edwards-deming]]**'s quality management: statistical process control, the distinction between common and special cause variation, the PDSA improvement cycle

Anderson's original contribution is the synthesis: applying these manufacturing and quality management ideas to knowledge work through the specific mechanism of WIP-limited visual workflow, packaged as an evolutionary overlay rather than a disruptive replacement.

## Origins at Corbis

The method crystallized during the [[corbis-kanban-experiment]] (January 2007), where Anderson was managing software teams. A team member suggested a whiteboard card wall to make work visible; [[dragos-dumitriu]] and [[rick-garber]] were early implementers. The concept of [[classes-of-service]] emerged when Drew McLean (VP) asked for an expedite capability. The core practices were being practiced before they were fully theorized; [[kanban-book]] (2010) provided the retrospective systematization.

## The Method as Change Management

Anderson consistently described the Kanban Method not as a software development methodology but as a **change management approach**. The board and WIP limits are diagnostic instruments as much as operational tools: they make dysfunction visible so it can be addressed. The evolutionary philosophy means change happens at the organization's own pace, responding to the signals the system provides — rather than to an external transformation timeline.

This framing influenced how the method was positioned relative to Lean and Agile: in [[kanban-alternative-path-to-agility]], Anderson argued that Kanban provides a pragmatic path to agility that avoids the organizational disruption and adoption failure common in Scrum implementations.
