---
id: deliver-as-fast-as-possible
title: Deliver as Fast as Possible
type: concept
tags:
- lean-software-development
- seven-lean-principles
- flow
- pull-systems
- cycle-time
- tps-translation
links:
- target: one-piece-flow
  relation: translates
  note: Small batch delivery principle from TPS one-piece flow
  kb: tps
- target: cost-of-delay
  relation: influenced_by
  note: Reinertsen's economic framework for why delivery speed matters
  kb: reinertsen
- target: queueing-theory-applied
  relation: influenced_by
  note: Mathematical foundation for why WIP limits improve flow
  kb: reinertsen
- target: batch-size-reduction
  relation: influenced_by
  note: Batch size economics underlying small-batch delivery
  kb: reinertsen
- target: drum-buffer-rope
  relation: related_to
  note: TOC's pacing mechanism parallels lean pull/flow
  kb: goldratt
- target: tempo
  relation: related_to
  note: Boyd's tempo — operating at faster cycle time than the opponent
  kb: boyd
importance: 8
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: pull systems, just-in-time (JIT), single-piece flow
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- seven-lean-principles
- pull-systems-in-software
- amplify-learning
- eliminate-waste
- optimize-the-whole
- value-stream-mapping-for-software
research_status: draft
---

Deliver as fast as possible is Principle 4 of the [[seven-lean-principles]], introduced by [[mary-poppendieck]] and [[tom-poppendieck]] in [[lean-software-development-agile-toolkit-2003]]. Its TPS sources are pull systems, just-in-time delivery, and single-piece flow — the cluster of techniques by which [[taiichi-ohno]] eliminated inventory buildup and made Toyota's production process responsive to actual demand.

## The TPS Foundation: Pull and JIT

[[taiichi-ohno]]'s insight at Toyota was that traditional "push" production — building to forecast, accumulating inventory — was fundamentally wasteful. Inventory is waste: it represents capital tied up in unfinished goods, it hides defects, and it decouples producers from the signals of actual demand. The alternative is a *pull* system: downstream processes signal their need to upstream processes, and production is triggered by actual consumption rather than forecast.

Just-in-time (JIT) is the operational expression of pull: parts arrive when and where they are needed, no sooner, in exactly the quantity required. Single-piece flow — moving one unit at a time through the production process rather than batching — is the extreme application of JIT, and it dramatically reduces cycle time and exposes defects immediately.

## Translation to Software

The Poppendiecks translated pull and JIT into software delivery. The software equivalent of inventory is partially done work: features that are coded but not integrated, tested but not deployed, deployed but not released. Like manufacturing inventory, partially done software work hides defects, ties up team capacity, and delays the feedback that would reveal whether the work was correct.

Fast delivery means small batches, short cycles, and frequent releases. The goal is to minimize the amount of work-in-progress at any stage — the software equivalent of JIT. [[pull-systems-in-software]] is the detailed treatment of how this applies to software work queues.

## Speed Serves Learning, Not Just Customers

A naive reading of "deliver as fast as possible" treats it as a customer satisfaction principle: customers want their software sooner. The Poppendiecks' deeper argument, consistent with [[amplify-learning]], is that speed serves the learning cycle. Fast delivery means fast feedback. Fast feedback means faster correction of wrong assumptions and faster incorporation of new knowledge. The competitive advantage of speed is primarily epistemic, not just commercial.

This is why delivery speed is a *lean* principle rather than simply an agile one. Speed is not about working harder or cutting corners. It is about removing the delays, batches, and handoffs that slow the flow of learning.

## Queueing Theory: Reinertsen's Contribution

[[donald-reinertsen]]'s work on product development flow provided the mathematical foundation for why speed matters that the Poppendiecks cited in [[implementing-lean-software-development-2006]]. Queueing theory, originally developed for telecommunications networks, shows that as utilization of a resource approaches 100%, queue lengths and wait times increase nonlinearly — a system at 80% utilization has dramatically shorter queues than one at 95% utilization. The implication for software teams is that maintaining capacity slack is not waste; it is the condition for responsiveness.

Reinertsen also formalized the *cost of delay* — the economic value destroyed by not delivering sooner. Making this cost visible transforms the conversation about speed from a productivity discussion to a business value discussion.

## Relationship to Continuous Delivery

Deliver as fast as possible is the principle that most directly influenced what became continuous delivery. [[gene-kim]]'s work on DevOps, and Jez Humble's continuous delivery research, both draw on the lean insight that deployment pipelines should minimize batch size and cycle time. The technical practices of continuous integration, automated testing, and deployment pipelines are engineering implementations of the pull and flow principles the Poppendiecks translated from TPS.

[[value-stream-mapping-for-software]] is the diagnostic tool for identifying where delays and batches accumulate in the delivery pipeline, making it the practical partner to this principle.
