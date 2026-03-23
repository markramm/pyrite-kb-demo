---
id: weighted-shortest-job-first
title: "Weighted Shortest Job First (WSJF)"
type: concept
importance: 8
tags:
- prioritization
- scheduling
- economics
- wsjf
- sequencing
first_appeared: "principles-of-product-development-flow"
key_writings:
- principles-of-product-development-flow
related_concepts:
- cost-of-delay
- economic-framework-for-prioritization
- u-curve-optimization
research_status: draft
---

Weighted Shortest Job First (WSJF) is a scheduling rule that achieves mathematically optimal sequencing of work items to minimize total delay cost across the portfolio. It is derived directly from [[cost-of-delay]] and duration, and it is the primary operational prescription of [[economic-framework-for-prioritization]].

## The Formula and Its Logic

WSJF = Cost of Delay / Job Duration

The rule: sequence jobs in descending order of this ratio. Do the job with the highest cost-of-delay per unit duration first.

The mathematical optimality of this rule follows from a classical result in scheduling theory. Given a set of jobs, each with a delay cost rate (cost per unit time of being undelivered) and a duration, the sequence that minimizes total weighted completion time is precisely the one that processes jobs in decreasing order of delay-cost-rate divided by duration. This is the "weighted shortest processing time" (WSPT) rule from operations research, applied to product development by Reinertsen under the WSJF label.

## Why It Matters

Without an explicit economic prioritization rule, teams default to heuristics: highest urgency (as perceived by the loudest stakeholder), largest feature (most visible), or first in first out. These heuristics do not minimize delay cost — they optimize for other things (political satisfaction, apparent productivity, simplicity). WSJF replaces these heuristics with a rule that provably minimizes total delay cost across the portfolio.

The key insight is that two jobs with the same cost of delay should be sequenced by duration — do the shorter one first, because it frees up capacity sooner and starts delivering its delay-cost savings earlier. Doing the longer job first means both jobs are delayed longer than necessary in aggregate.

## Connection to Cost of Delay

WSJF is mechanically dependent on [[cost-of-delay]] estimates. If delay costs are not quantified, WSJF cannot be computed. This is why Reinertsen treats cost of delay as the foundational concept: it is the input that makes optimal scheduling possible. WSJF is the mechanism; cost of delay is the economic substance.

## SAFe Adoption and Simplification

[[dean-leffingwell]]'s Scaled Agile Framework (SAFe) adopted WSJF as a prioritization mechanism, making it accessible to a much larger audience. However, SAFe's implementation modified the formula: rather than estimating cost of delay directly (which requires business analysis), SAFe substitutes a composite proxy score derived from user-business value, time criticality, and risk reduction / opportunity enablement. Duration is proxied by "job size" in story points.

This simplification trades precision for accessibility. Reinertsen's version requires actually estimating delay costs in economic terms; SAFe's version uses relative scoring that avoids explicit dollar estimates. The result is easier to implement but loses the mathematical grounding that makes the original rule provably optimal. Reinertsen has noted this trade-off explicitly.

## Lineage

The mathematical optimality result traces to scheduling theory developed in operations research in the 1950s-70s (Smith, 1956; Conway, Maxwell, Miller, 1967). Reinertsen's contribution was recognizing that this classical result applies to product development prioritization and constructing the cost-of-delay framing that makes the rule practically computable.
