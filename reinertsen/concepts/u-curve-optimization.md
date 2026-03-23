---
id: u-curve-optimization
title: "U-Curve Optimization"
type: concept
importance: 9
tags:
- economics
- trade-off
- optimization
- batch-size
- u-curve
first_appeared: "managing-the-design-factory"
key_writings:
- managing-the-design-factory
- principles-of-product-development-flow
related_concepts:
- economic-framework-for-prioritization
- batch-size-reduction
- managing-variability
- wip-constraints
- cost-of-delay
research_status: draft
---

The U-curve is a recurring structural insight in Reinertsen's work: for most important parameters in product development — batch size, WIP level, testing coverage, process formality — both extremes are costly, and the optimal value lies somewhere in between. Recognizing this pattern distinguishes an economic approach from dogmatic thinking, whether that dogma favors lean minimalism or traditional heavyweight process.

## The Basic Structure

A U-curve arises whenever a parameter simultaneously drives two costs in opposite directions:

- One cost decreases as the parameter increases (e.g., transaction costs per unit decrease as batch size grows)
- Another cost increases as the parameter increases (e.g., holding costs grow as batch size grows)

The total cost — the sum of these two curves — forms a U shape with a minimum at some intermediate value. That minimum is the economic optimum. Moving away from the optimum in either direction increases total cost.

## Why This Matters for Practice

The U-curve insight has a direct prescriptive consequence: blanket rules like "always do X" or "X is waste" are wrong if X has a U-curve. The correct rule is "optimize X given your current cost structure."

This distinguishes Reinertsen from dogmatic lean thinking. Lean traditions (drawing on [[taiichi-ohno]]'s TPS) often treat batch size reduction, inventory reduction, and WIP reduction as absolute goods — more reduction is always better. Reinertsen's analysis shows this is only true when transaction costs are near zero. When transaction costs are real (e.g., integration is expensive, testing is slow, deployment is risky), the optimal batch size is greater than one. The correct response is to reduce transaction costs — moving the curve's minimum — not to operate below the current optimum on ideological grounds.

## Recurring Instances in Reinertsen's Work

**Batch size** ([[batch-size-reduction]]): Transaction cost vs. holding cost. Optimal batch minimizes their sum. Reducing transaction costs (automation, tooling) shifts the optimum toward smaller batches.

**WIP level** ([[wip-constraints]]): Capacity cost of idle workers vs. [[cost-of-delay]] from queues. Optimal WIP level maintains some slack rather than maximizing utilization.

**Variability** ([[managing-variability]]): Eliminating variability has costs (reduced exploration, less innovation opportunity). Some variability is valuable. The optimal level is not zero.

**Process formality**: Too little process creates coordination failures; too much creates bureaucratic overhead. The optimum is an intermediate level of formality matched to task uncertainty and team size.

**Testing coverage**: Too little testing misses defects; too much testing delays delivery. Cost of escaped defects vs. cost of testing time.

## Relationship to Economic Framework

The U-curve is the structural form that [[economic-framework-for-prioritization]] takes in practice. Rather than applying fixed rules, the economic framework asks: what are the costs on both sides of this decision? Where do they cross? That analysis, repeated across all the parameters of product development, produces the U-curve pattern. Reinertsen's contribution was making this pattern explicit and showing that it applies across an unusually wide range of product development decisions.

## Lineage

U-curve optimization is standard in operations research and economics — the Economic Order Quantity model (Harris, 1913), newsvendor problems, and queueing capacity planning all use it. Reinertsen's contribution was applying this framework systematically to knowledge work and using it to critique both traditional heavyweight processes and lean-derived minimalism.
