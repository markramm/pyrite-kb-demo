---
id: value-stream-mapping-for-it
title: "Value Stream Mapping for IT"
type: concept
importance: 6
tags:
- lean
- flow
- value-stream
- bottleneck
- lead-time
- waste
concept_type: pattern
first_appeared: "Adapted from lean manufacturing; applied to IT in The DevOps Handbook (2016)"
key_writings:
- the-devops-handbook
- the-phoenix-project
related_concepts:
- three-ways
- deployment-pipeline
- continuous-delivery
research_status: draft
---

Value stream mapping for IT is the practice of visualizing the complete flow of work from business request to production deployment, identifying every step, every wait, and every handoff — to reveal where time is lost and where improvement will have the most impact.

## Lean Origins

Value stream mapping originated in lean manufacturing, descended from Toyota's material and information flow mapping practices. Mary and Tom Poppendieck adapted it for software in "Lean Software Development" (2003), establishing the conceptual vocabulary: value-adding steps, non-value-adding steps, wait time, work time, lead time, cycle time.

The adaptation required reconceptualizing what "the product" is. In manufacturing, you map the physical flow of materials. In software delivery, you map the flow of information: a business requirement becoming a feature request becoming a work item becoming code becoming a test result becoming a deployment becoming a production capability. The product is intangible but the delays are very real.

## The Key Insight: Wait Time Dominates

When organizations map their IT value streams for the first time, the finding is almost always the same: the vast majority of lead time — the time from idea to production — is wait time, not work time. Code review queues. Approval processes for change management boards. Test environment provisioning. Security scans awaiting a security team slot. Deployment windows that happen once a week.

[[the-devops-handbook]] illustrates this with examples where 90%+ of calendar time is spent waiting, not performing value-adding work. A feature that takes two days of actual engineering work might take six weeks to reach production because of queues at handoffs.

This connects to Goldratt's Theory of Constraints: the value stream has a constraint — the bottleneck step that limits throughput. All other improvement efforts are subordinate to identifying and addressing that constraint. The [[three-ways]] first way is about making the flow visible precisely so the constraints can be seen.

## The Teaching Function

[[the-phoenix-project]] uses value stream mapping as its central teaching device. The novel's protagonist, Bill Palmer, is introduced to the concept through a plant tour with Erik, a mentor figure modeled on lean and TOC principles. Erik shows Bill the manufacturing plant's visual management — boards showing flow, queues, and constraints — and asks him to find the equivalent in IT.

The answer is the value stream map: the equivalent of the plant floor, where work in process becomes visible, wait times are exposed, and constraints emerge from the data rather than from organizational politics. The novel's dramatic arc is largely Bill learning to see his organization's value stream and act on what he sees.

## Connection to DORA Metrics

[[dora-four-key-metrics]] — particularly Lead Time for Changes — is a value stream metric. Lead time for changes measures the time from code commit to running in production: the duration of the software delivery value stream's critical path. Improving lead time for changes means removing the waste and wait from the value stream.

[[accelerate-book]] demonstrates that organizations with short lead times (high performers: less than one hour) have fundamentally different value streams than organizations with long lead times (low performers: one to six months). The structural difference is not in the quality of individual engineers but in how the value stream is organized: the number of handoffs, the size of batches, the presence or absence of automation at bottleneck steps.

## Deployment Pipeline as Value Stream Tool

The [[deployment-pipeline]] concept from [[continuous-delivery-book]] is the implementation of value stream thinking in software delivery tooling. A deployment pipeline makes the software delivery value stream visible and executable: every step from code commit to production deployment is defined, automated, and instrumented. Wait times become measurable. Bottlenecks become visible. The pipeline IS the value stream map, made operational.

## Relationship to Kanban

Kanban boards — widely adopted in software teams — are a partial value stream visualization. A kanban board shows work items moving through defined stages and exposes work in process. But most kanban implementations cover only the development phase. Value stream mapping for IT extends the view through operations to production: the full delivery chain, not just the development portion. [[the-devops-handbook]] emphasizes this extension as essential to DevOps thinking.
