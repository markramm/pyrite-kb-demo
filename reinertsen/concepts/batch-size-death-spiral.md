---
id: batch-size-death-spiral
title: Batch Size Death Spiral
type: concept
tags:
- batch-size
- anti-pattern
- reinforcing-loop
importance: 7
first_appeared: principles-of-product-development-flow
key_writings:
- principles-of-product-development-flow
related_concepts:
- batch-size-reduction
- cost-of-delay
- u-curve-optimization
- economic-framework-for-prioritization
research_status: draft
---

The Batch Size Death Spiral is a reinforcing feedback loop described in [[principles-of-product-development-flow]] where large batches create conditions that make batches even larger. The mechanism: large projects attract additional scope ("while we're at it, let's also..."), additional cost justification (large overhead costs must be amortized over more features), additional review cycles, and additional stakeholder involvement. Each addition makes the batch larger, which attracts more additions — a classic positive feedback loop.

This concept illustrates Reinertsen's application of systems thinking to product development economics. The death spiral is the opposite of the virtuous cycle created by [[batch-size-reduction]]: smaller batches reduce overhead per transaction, reduce queue time, accelerate [[fast-feedback]], and make it economically rational to keep batches small. The spiral breaks when organizations recognize that transaction costs — the costs of processing a batch (testing, deployment, review) — are the lever. Reducing transaction costs shifts the [[u-curve-optimization]] toward smaller optimal batch sizes.

The death spiral also connects to [[cost-of-delay]]: large batches delay everything in the batch by the duration of the slowest item. The delay cost compounds across all items in the batch, but because delay cost is typically invisible (one of Reinertsen's central observations), organizations don't see the damage large batches cause.
