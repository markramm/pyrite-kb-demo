---
id: queueing-theory-applied
title: Queueing Theory Applied to Product Development
type: concept
tags:
- queueing-theory
- mathematics
- flow
- wip
- variability
links:
- target: statistical-process-control-and-variation-theory
  relation: builds_on
  note: Reinertsen's queueing theory extends Deming's variation theory — variability
    in arrivals and service times is what drives queue formation, connecting SPC insight
    to flow economics
  kb: deming
- target: drum-buffer-rope
  relation: related_to
  note: Reinertsen's queueing theory and Goldratt's drum-buffer-rope both address
    managing flow through a system with a binding constraint — different formalisms,
    convergent insights
  kb: goldratt
importance: 10
first_appeared: managing-the-design-factory
key_writings:
- managing-the-design-factory
- principles-of-product-development-flow
related_concepts:
- wip-constraints
- batch-size-reduction
- managing-variability
- flow-control
- cost-of-delay
research_status: draft
---

Queueing theory — the branch of operations research concerned with waiting lines, service rates, and utilization — is the mathematical foundation underlying most of Reinertsen's prescriptive recommendations. Introduced in [[managing-the-design-factory]] and fully developed in [[principles-of-product-development-flow]], its application to product development explains phenomena that experience-based intuition consistently gets wrong.

## The Key Mathematical Results

**Little's Law** (attributed to [[john-little]], 1961) states that in any stable system, the average number of items in the system equals the average arrival rate multiplied by the average time each item spends in the system: L = λW. In product development terms: Work in Process = Throughput × Cycle Time. This is an identity — it holds regardless of queue discipline, arrival distribution, or service distribution. Its implication is that reducing WIP directly reduces cycle time at constant throughput.

**The M/M/1 Queue** (single server, exponential arrivals, exponential service times) provides the baseline model for a single development resource. Its critical result: as utilization ρ approaches 1 (100%), average queue length grows without bound as ρ/(1-ρ). At 80% utilization, average queue length is 4x the in-service item. At 95%, it is 19x. The relationship is nonlinear and accelerating — this is why the last increment of capacity utilization is disproportionately costly in cycle time terms.

**Variability** compounds these effects. The Kingman equation (also called the VUT equation) expresses queue wait time as proportional to utilization, variability of arrivals, and variability of service times. High variability at high utilization produces extreme queues. This provides the mathematical basis for [[managing-variability]]: even if variability cannot be eliminated, reducing it has compounding benefits at high utilization.

## Why This Was New in Product Development

Manufacturing had applied queueing theory since the mid-20th century. Product development had not, in part because its queues are invisible — a queue of engineering tasks has no physical form, no floor space cost, no obvious holding cost. Reinertsen's contribution was making these invisible queues visible and attaching [[cost-of-delay]] to them, transforming an abstract mathematical concern into a business economics argument.

## Practical Implications

The queueing results explain several counterintuitive behaviors:

- Adding capacity at high utilization produces disproportionate cycle-time improvement because the system is operating in the nonlinear region of the utilization-queue curve
- Reducing variability at high utilization is more valuable than reducing it at low utilization
- [[batch-size-reduction]] reduces both average queue length and queue variability
- [[wip-constraints]] prevent the system from entering the dangerous high-utilization region

These implications form the technical backbone for Kanban WIP limits as later systematized by [[david-anderson]], who drew directly on Reinertsen's queueing analysis.

## Lineage

The mathematical tools originate in teletraffic engineering (Erlang, 1909) and were formalized in the mid-20th century by Kendall, Jackson, and Little. Reinertsen's synthesis applies these results to knowledge work, analogizing development tasks to service requests and development teams to service channels. The key conceptual move — treating product development as a queueing system rather than a planning problem — reframes the entire discipline.
