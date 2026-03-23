---
id: flow-principle
title: "Flow (Third Lean Principle)"
type: concept
importance: 8
tags:
- lean-thinking
- five-principles
- continuous-flow
- batch-elimination
first_appeared: "Lean Thinking (1996)"
key_writings:
- lean-thinking
- beyond-toyota
related_concepts:
- five-lean-principles
- value-stream-principle
- pull-principle
- lean-production
tps_source: "TPS one-piece flow and elimination of batch-and-queue — the operational heart of Toyota's production method"
application_domain: general
research_status: draft
---

The third of the [[five-lean-principles]]: make the value-creating steps flow continuously. Once [[value-principle|value]] is defined and the [[value-stream-principle|value stream]] mapped, the next step is to make work flow through the remaining value-creating steps without interruption, backflow, waiting, or scrap.

## The Principle

[[james-p-womack]] and [[daniel-t-jones]] argue in [[lean-thinking]] that the natural tendency of organizations is to batch work — process large lots through each department before passing them to the next. Batching creates queues, waiting, inventory, and the illusion of efficiency (each department looks busy) while the overall system is slow and wasteful.

Flow means moving from batch-and-queue to continuous, one-piece (or small-lot) processing. The ideal is that each unit of work moves immediately to the next value-creating step without waiting.

## TPS Source

This is the closest of the five principles to the operational heart of [[taiichi-ohno]]'s TPS. One-piece flow was Toyota's defining production innovation: instead of building cars in large batches through each department, Toyota organized production cells where a single vehicle (or component) moved continuously through all operations. The result was faster throughput, smaller inventory, and immediate defect detection.

Ohno's flow was physical — the movement of parts through a factory. Womack and Jones abstracted "flow" to include information flow, design flow, and service delivery flow. This abstraction enabled application beyond manufacturing but also introduced metaphorical stretch: information doesn't "flow" the same way a car body moves through a paint booth.

## The Counterintuitive Insight

Womack and Jones emphasize that flow is counterintuitive to managers trained in mass production: it feels wrong to process one item at a time when you could "efficiently" batch hundreds. The revelation — documented through case studies in [[lean-thinking]] and [[beyond-toyota]] — is that total system performance improves dramatically when batch sizes shrink, even though individual process step efficiency may appear to decrease.

This insight about local optimization versus system optimization connects to Goldratt's Theory of Constraints and to Deming's systems thinking, though Womack and Jones frame it in lean vocabulary rather than citing those traditions directly.

## Downstream Adoption

The flow concept became one of the most widely adopted lean ideas:
- In software: continuous integration, continuous delivery, and the DevOps movement all draw on flow concepts
- In healthcare: patient flow through emergency departments and surgical pathways
- Csikszentmihalyi's psychological "flow state" is a coincidental parallel, not a borrowing — but the Lean/Agile community sometimes conflates the two

## Research Needed

- Whether Womack/Jones drew explicitly on queuing theory or operations research for their flow arguments
- The relationship between lean flow and Goldratt's throughput-focused thinking in Theory of Constraints
