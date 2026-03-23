---
id: flow-control
title: Flow Control
type: concept
tags:
- flow
- wip
- pull-systems
- queue-management
- economics
links:
- target: system-of-profound-knowledge
  relation: builds_on
  note: Reinertsen's flow-based product development framework builds on Deming's appreciation
    for a system — both reject local optimization in favor of end-to-end throughput
  kb: deming
- target: deliver-as-fast-as-possible
  relation: related_to
  note: Reinertsen's flow control principles provide the quantitative mechanics behind
    the Poppendiecks' 'deliver as fast as possible' lean principle
  kb: poppendiecks
importance: 7
first_appeared: principles-of-product-development-flow
key_writings:
- principles-of-product-development-flow
related_concepts:
- wip-constraints
- queueing-theory-applied
- cadence-and-synchronization
- batch-size-reduction
- cost-of-delay
research_status: draft
---

Flow control is the active management of work state in a product development process — regulating the rate and volume of work entering, progressing through, and exiting the system to maintain predictable cycle times and minimize [[cost-of-delay]]. In Reinertsen's framework, "flow" carries a specific technical meaning distinct from both its colloquial use and its use in positive psychology.

## Disambiguating "Flow"

The term flow in product development literature is used in at least three different senses:

1. **Reinertsen's flow** (this concept): economic flow state — work moving through a development system at a rate that minimizes total delay cost, achieved through WIP constraints, pull systems, and queue management
2. **Csikszentmihalyi's flow**: the psychological state of optimal engagement and absorption in a task — related to individual productivity but not directly to system throughput
3. **Lean flow**: the ideal state where products move continuously through production without waiting — the Toyota concept of one-piece flow

Reinertsen's flow control is primarily about the first sense, though it is informed by lean flow concepts. The goal is not psychological flow for individuals (though that may be beneficial) but economic flow for the system — work completing at predictable rates with minimal queue buildup.

## Mechanisms of Flow Control

**Pull vs. Push**: Push systems release work into the process as it arrives (demand-driven). Pull systems release work only when downstream capacity is available (capacity-driven). Pull systems maintain predictable WIP and cycle times; push systems allow WIP to grow without bound when demand exceeds capacity. [[wip-constraints]] implemented as pull systems are the primary flow control mechanism.

**Queue management**: Active monitoring of queue lengths at each process stage and intervention when queues grow. The queueing results from [[queueing-theory-applied]] provide the theoretical basis: queues at high utilization grow exponentially, so early intervention at moderate queue lengths is more effective than attempting to drain large queues.

**Arrival rate control**: Throttling the rate at which new work enters the system to match throughput capacity. Without arrival rate control, a backlogged system will never clear its queues because new work arrives faster than old work is completed.

## Connection to WIP Constraints

[[wip-constraints]] are the primary operational tool of flow control — the mechanism by which the system is kept in the linear, predictable region of the utilization-queue curve. Flow control is the broader concept; WIP constraints are its primary implementation.

## Cadence as Flow Regularity

[[cadence-and-synchronization]] contributes to flow control by regularizing the timing of work releases and integrations. A regular cadence converts bursty, variable arrivals into more uniform flow, reducing the variability component of queue buildup (as described by the Kingman equation in [[queueing-theory-applied]]).

## Economic Objective

The economic objective of flow control is minimizing total [[cost-of-delay]] across the portfolio while maintaining acceptable utilization of development capacity. This is a queueing optimization problem: find the operating point on the utilization curve that minimizes total cost (delay cost plus capacity cost). Flow control mechanisms are the operational tools for reaching and maintaining that operating point.
