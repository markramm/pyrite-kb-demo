---
id: one-piece-flow
title: One-Piece Flow
type: concept
tags:
- flow
- batch-size
- production
- core-principle
links:
- target: batch-size-reduction
  relation: influenced
  note: TPS one-piece flow is the canonical demonstration that batch size reduction
    improves cycle time and quality — the empirical foundation for Reinertsen's batch-size
    theory
  kb: reinertsen
importance: 7
first_appeared: Developed by Ohno at Toyota, 1950s-1960s
related_concepts:
- just-in-time
- smed
- takt-time
- pull-production
- value-stream
research_status: draft
---

Processing one item at a time through the entire production sequence, rather than processing a batch at each station before moving the batch forward. One-piece flow minimizes work-in-progress inventory, makes defects immediately visible (the next station catches the problem within seconds, not hours), and dramatically reduces lead time. [[taiichi-ohno]]'s early experiments with [[ohno-begins-multi-machine-experiments|multi-machine operation]] were the genesis of one-piece flow — a single worker operating multiple machines in sequence rather than a batch operator at a single machine. One-piece flow requires balanced workstations ([[takt-time]]), reliable processes ([[jidoka]]), fast changeover ([[smed]]), and small lot sizes. It is the manufacturing embodiment of "small batches" that appears in every lean methodology downstream — from continuous integration in software to the minimum viable product in Lean Startup.
