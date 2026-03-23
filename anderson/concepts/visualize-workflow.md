---
id: visualize-workflow
title: "Visualize Workflow"
type: concept
tags:
- core
- visual-management
- kanban-board
- transparency
links:
- target: andon
  relation: related_to
  note: Kanban boards make workflow problems visible in real time — the knowledge-work equivalent of Toyota's andon visual management system
  kb: tps
- target: office-environment-effect
  relation: related_to
  note: 'Both address making invisible dynamics visible: DeMarco showed the invisible cost of poor office environments; Anderson makes invisible workflow problems visible on the board'
  kb: demarco
importance: 8
metadata:
  first_appeared: "corbis-kanban-experiment"
  key_writings: &id001
  - kanban-book
  - essential-kanban-condensed
  - corbis-kanban-presentation
  related_concepts: &id002
  - kanban-method
  - wip-limits
  - manage-flow
  - make-policies-explicit
  - classes-of-service
  source_tradition: "TPS (visual management, kanban cards)"
  research_status: draft
first_appeared: "corbis-kanban-experiment"
key_writings: *id001
related_concepts: *id002
source_tradition: "TPS (visual management, kanban cards)"
research_status: draft
---

Visualize Workflow is the first of the six core practices of Anderson's [[kanban-method]]: making work, workflow stages, and Work in Progress visible — typically on a physical or digital board where cards represent work items and columns represent workflow states.

## Origins at Corbis

The practice has a specific origin point. During the [[corbis-kanban-experiment]] in January 2007, Anderson was managing software teams at Corbis. A team member — accounts vary on who first proposed it — suggested putting work on a whiteboard. Darren Davis, the team's manager, implemented the first card wall. Anderson recognized the significance immediately: making invisible knowledge work visible was the prerequisite for every subsequent management intervention.

This origin matters because it illustrates a recurring pattern in the Kanban Method's development: practices emerged from practical necessity in real teams before they were systematized into a framework. The Corbis board was not designed from theory; it was a response to a coordination problem.

## What Gets Visualized

A well-designed Kanban board makes several things visible simultaneously:

- **Work items** (cards), each representing a unit of value to be delivered
- **Workflow stages** (columns), representing the states work passes through from request to delivery
- **WIP** — how many items are currently active in each stage
- **Blockers** — work that cannot progress (typically marked visually, e.g., a red dot or sticky)
- **[[classes-of-service]]** — the urgency/risk category of each item (often indicated by card color)
- **Age** — how long an item has been in its current state, making aging work visible

The board's design is not prescribed by the Kanban Method. Anderson consistently argued that the board should reflect the actual workflow of the team, not an idealized or imported model. This is an expression of the [[evolutionary-change]] principle: start with what you do now, visualize it accurately, then improve.

## Relationship to Toyota's Visual Management

[[taiichi-ohno]]'s Toyota Production System used visual management extensively: production status boards, andon cords, status lights, inventory kanban cards. The principle — that problems should be immediately visible rather than hidden — translates directly. Anderson borrowed the kanban card as a work item signal and the visual pull logic, but adapted the form for knowledge work where the "inventory" is ideas, tasks, and partially completed software rather than physical parts.

The important distinction: Toyota's kanban cards were physical scheduling tokens that triggered production. Anderson's kanban cards are information radiators that make the state of knowledge work visible to the whole team. The visual management purpose is shared; the mechanism is adapted for a fundamentally different type of work.

## Why Visualization Precedes Other Practices

In Anderson's formulation, visualization is listed first among the six practices because it is the prerequisite for all others. You cannot impose meaningful [[wip-limits]] on work you cannot see. You cannot [[manage-flow]] without knowing what is flowing. You cannot [[make-policies-explicit]] about a system you haven't mapped. The board is not decoration; it is the instrument through which the system becomes legible.

The [[statik]] methodology formalizes this: one of the early steps in designing a kanban system is to map the actual workflow — often discovering that the organization's formal process description and the real workflow are significantly different. The board reflects reality, not the org chart.

## Board Design Considerations

[[kanban-book]] discusses board design through case studies from Corbis and other engagements. Key design decisions include:

- **Column granularity.** Too few columns obscure where work ages; too many create administrative overhead.
- **Queue vs. active columns.** Some implementations distinguish "waiting" columns (buffer queues) from "active" columns (someone is actively working on items here). This enables WIP limits to distinguish between active processing and waiting.
- **Swim lanes.** Horizontal lanes can separate [[classes-of-service]] or work types, allowing different flow policies to coexist on the same board.
- **Buffer columns.** A column between two stages that represents a handoff queue — making the hand-off visible and measurable.

Anderson's later work with [[statik]] and the [[kanban-maturity-model-concept]] addressed how board design evolves as organizational maturity increases: early boards are simple, later boards may have multiple services, swim lanes, and explicit buffer management.
