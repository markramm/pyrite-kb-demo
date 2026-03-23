---
id: drum-buffer-rope
title: Drum-Buffer-Rope
type: concept
tags:
- production-scheduling
- operations
- flow-management
links:
- target: flow-control
  relation: related_to
  note: DBR is a WIP-constraining flow mechanism; Reinertsen's flow control and WIP
    constraints derive similar logic from queuing theory
  kb: reinertsen
importance: 8
first_appeared: The Race (1986)
key_writings:
- the-goal
- the-race
- theory-of-constraints-book
related_concepts:
- theory-of-constraints
- five-focusing-steps
- buffer-management
- throughput-accounting
- critical-chain-project-management
research_status: draft
---

Drum-Buffer-Rope (DBR) is [[eliyahu-goldratt]]'s production scheduling method, designed to operationalize the [[five-focusing-steps]] on the shop floor. It provides a concrete mechanism for subordinating the entire production system to the pace of its constraint.

The three elements:

- **Drum:** The constraint resource, which sets the beat (the drum) for the entire system. The production schedule is built around maximizing the constraint's utilization on the right work.
- **Buffer:** A time buffer of work placed immediately in front of the constraint. The buffer protects the constraint from starvation caused by the natural variability of upstream operations — it ensures the constraint is never idle waiting for materials.
- **Rope:** A communication mechanism that ties raw material release at the front of the plant to the constraint's consumption rate. The rope limits work-in-process (WIP) and prevents the buildup of inventory upstream of the constraint.

DBR was first described concretely in [[the-race]] (1986), co-authored with [[robert-fox]], which presented the underlying production logic in a more structured form than [[the-goal]]'s narrative. DBR directly challenges the conventional wisdom that every resource should be kept busy — idle non-constraint capacity is often desirable, not wasteful, because excess production simply becomes stranded inventory.

[[buffer-management]] is DBR's ongoing monitoring companion: rather than tracking machine utilization, managers watch how buffer levels fluctuate, using buffer penetration as the signal for when to intervene.

A simplified variant, Simplified DBR (S-DBR), was later developed to handle environments where the constraint is the market rather than an internal resource, and was explored by [[eli-schragenheim]] and others in the [[avraham-y-goldratt-institute]] community.
