---
id: managing-variability
title: Managing Variability
type: concept
tags:
- variability
- queueing-theory
- buffers
- economics
- lean
links:
- target: common-cause-vs-special-cause-variation
  relation: builds_on
  note: Reinertsen's variability management framework extends Deming's common vs.
    special cause distinction into the economics of buffering, pooling, and reducing
    variation
  kb: deming
importance: 8
first_appeared: managing-the-design-factory
key_writings:
- managing-the-design-factory
- principles-of-product-development-flow
related_concepts:
- queueing-theory-applied
- u-curve-optimization
- wip-constraints
- batch-size-reduction
- fast-feedback
principle_numbers: V1-V16
research_status: draft
---

Variability in product development should be managed, not eliminated — unlike in manufacturing. This is one of Reinertsen's most important points of departure from lean orthodoxy: the economic case for variability reduction is context-dependent, and some variability is deliberately valuable. Principle numbers V1-V16 in [[principles-of-product-development-flow]].

## The Lean Manufacturing Starting Point

Lean manufacturing, derived from [[taiichi-ohno]]'s Toyota Production System, treats variability as pure waste. Mura (unevenness) is one of the three sources of waste in TPS, alongside Muda (non-value-adding activity) and Muri (overburden). In a manufacturing context with highly repetitive, well-understood processes, this is economically correct: variability reduces throughput, increases inventory, and creates defects without producing any compensating benefit.

## Why Product Development Is Different

Product development is an information-creation process, not a physical transformation process. Its purpose is to discover something new — a design, a feature, a market insight — that did not exist before. This discovery process is inherently variable: good ideas and bad ideas, successful experiments and failed experiments, customer responses that confirm assumptions and responses that overturn them.

Some of this variability is economically valuable. An exploratory design process that generates multiple divergent concepts and then selects the best one exploits variability — the value comes precisely from the spread of outcomes and the ability to select from among them. Eliminating variability in this context would mean pursuing only one design concept, which removes the possibility of discovering a better solution.

This is the key distinction: manufacturing variability is symmetric (random fluctuation around a target is never helpful); product development variability is asymmetric (you can select the right tail, making high variance in good directions valuable).

## The Queueing Consequence

While some variability is valuable, variability has real costs in queueing terms. From [[queueing-theory-applied]], the Kingman equation shows that queue wait time is proportional to the variability of both arrivals and service times (as well as utilization). High variability at high utilization produces extreme, unpredictable queues. This creates [[cost-of-delay]] through unpredictable cycle times.

The economic framework therefore calls for managing variability's consequences rather than eliminating variability itself. The tools are:

- **Buffers**: capacity buffers (slack time), inventory buffers (partially completed work), and schedule buffers absorb variability at the cost of holding cost
- **[[wip-constraints]]**: limit how much variability can accumulate in the system at once
- **[[batch-size-reduction]]**: smaller batches reduce the impact of individual variable outcomes
- **[[fast-feedback]]**: faster cycles mean errors from high variability are caught and corrected sooner

## The U-Curve of Variability Management

This is another instance of [[u-curve-optimization]]: too much variability management (eliminate all variability) destroys the exploration value of product development; too little variability management allows queue explosion and unpredictable cycle times. The optimum preserves beneficial variability (exploration, innovation) while managing the queueing consequences of variability through buffers and WIP constraints.

## Distinguishing Beneficial from Harmful Variability

Reinertsen distinguishes variability by its source and selectability:
- **Beneficial variability**: outcomes where you can select the best (design alternatives, prototyping options, market tests) — exploit this
- **Harmful variability**: outcomes where you cannot select (task completion times, defect arrival rates, dependency delays) — buffer or reduce this

Principle V1-V16 operationalizes this distinction with specific prescriptions for each type.
