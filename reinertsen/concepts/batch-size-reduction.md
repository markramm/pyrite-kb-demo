---
id: batch-size-reduction
title: Batch Size Reduction
type: concept
tags:
- batch-size
- flow
- feedback
- u-curve
- lean
links:
- target: one-piece-flow
  relation: builds_on
  note: Reinertsen provides the economic theory for why one-piece flow works — his
    batch-size analysis shows the U-curve optimum and quantifies the transaction cost
    vs. holding cost tradeoff
  kb: tps
importance: 9
first_appeared: managing-the-design-factory
key_writings:
- managing-the-design-factory
- principles-of-product-development-flow
related_concepts:
- u-curve-optimization
- fast-feedback
- queueing-theory-applied
- wip-constraints
- managing-variability
principle_numbers: B1-B19
research_status: draft
---

Batch size — the quantity of work processed together before handoff or integration — is a fundamental lever in Reinertsen's flow framework. Reducing batch size improves cycle time, accelerates feedback, and reduces variability in queue lengths. The relationship is not monotonic, however: there is an optimal batch size governed by a [[u-curve-optimization]] trade-off, and understanding that curve is essential to applying the principle correctly.

## The Economic Trade-off

Batch size creates a classic two-sided cost structure:

**Transaction costs** (fixed costs per batch): setup time, coordination overhead, integration effort, context-switching cost. These costs are incurred once per batch regardless of size, so they decrease per unit as batch size grows. Larger batches amortize transaction costs more efficiently.

**Holding costs** (variable costs proportional to batch size): delayed feedback, inventory of unvalidated assumptions, queue buildup waiting for the next batch, risk accumulation. These costs grow with batch size. In product development, holding cost is primarily expressed through [[cost-of-delay]] — each item in the batch is waiting, and that wait has an economic cost.

The optimal batch size minimizes total cost — the sum of these two curves. This U-curve structure means both "always use smaller batches" and "always use larger batches" are wrong as absolute rules. The correct answer depends on the ratio of transaction costs to holding costs, which varies by organization, process maturity, and tooling.

## How Reducing Transaction Costs Changes the Optimum

A key insight: reducing transaction costs shifts the optimal batch size downward. When integration becomes cheaper (continuous integration tools, automated testing, deployment pipelines), the optimum moves toward smaller batches. This explains why lean and agile practices that invest in reducing transaction costs (e.g., test automation) enable — and justify — smaller batches. The investment in tooling changes the shape of the cost curve, not just the operations on a fixed curve.

## Queueing Effects

From [[queueing-theory-applied]], batch size affects queue dynamics in two ways. First, larger batches create larger queue entries, increasing average wait time for all items in the batch beyond the first. Second, batch processing creates bursty arrivals, increasing arrival variability and thus (via the Kingman equation) increasing average queue length. Smaller batches produce smoother, less variable flow.

## Feedback Acceleration

Smaller batches reach integration and validation faster. In a learning system — which product development always is — faster feedback means errors are corrected with less accumulated rework. This connects to [[fast-feedback]]: the economic value of feedback is a function of both its accuracy and its timeliness. An insight that arrives after a team has spent six weeks building on a flawed assumption is worth less than the same insight after one week.

## Principle Numbers B1-B19

Reinertsen dedicates 19 principles in [[principles-of-product-development-flow]] to batch size, more than any other single topic. This reflects his view that batch size is underappreciated as a control variable — most organizations manage resources, schedules, and scope, but rarely treat batch size as a deliberately optimized parameter.

## Lineage

The batch size trade-off analysis originates in inventory theory — the Economic Order Quantity model (Harris, 1913) applies exactly this U-curve logic to manufacturing. [[taiichi-ohno]]'s Toyota Production System applied batch reduction to manufacturing through single-piece flow and SMED (setup time reduction). Reinertsen's contribution was extending the economic analysis to product development, where the holding costs are informational rather than physical.
