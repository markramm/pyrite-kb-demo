---
id: pull-systems-in-software
title: Pull Systems in Software
type: concept
tags:
- lean-software-development
- kanban
- pull
- flow
- tps-translation
links:
- target: pull-production
  relation: translates
  note: Software pull systems translated from TPS pull production
  kb: tps
- target: kanban
  relation: translates
  note: Software kanban derived from TPS kanban signaling
  kb: tps
- target: wip-constraints
  relation: influenced_by
  note: WIP constraints as the mechanism for implementing pull
  kb: reinertsen
importance: 7
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: kanban (signaling system); pull production; just-in-time
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- deliver-as-fast-as-possible
- seven-lean-principles
- eliminate-waste
- value-stream-mapping-for-software
- optimize-the-whole
research_status: draft
---

Pull systems in software is the Poppendiecks' translation of [[taiichi-ohno]]'s kanban and pull production principles from the Toyota Production System into software delivery. Introduced in [[lean-software-development-agile-toolkit-2003]], this concept became one of the most influential in the lean software lineage, directly seeding [[david-anderson]]'s Kanban method for software and knowledge work.

## The TPS Foundation: Kanban and Pull

[[taiichi-ohno]] developed the kanban system at Toyota in the late 1940s as a mechanism for implementing pull production. In a push system, each production stage produces according to a schedule or forecast, pushing output to the next stage. Inventory accumulates wherever downstream stages cannot keep pace. In a pull system, each stage produces only what the downstream stage signals it needs, when it signals it. The kanban card (originally a physical card) is the signal: a downstream station sends a card upstream to authorize production of a specific item.

The result is dramatically reduced inventory. Work-in-process is limited to what the system is actively consuming. Problems propagate immediately — if a downstream station is blocked, the upstream station stops quickly, making the problem visible rather than hiding it behind buffer inventory.

[[taiichi-ohno]] drew the inspiration for pull production from American supermarkets, which replenished shelves based on actual sales rather than forecasts. The supermarket was his model of pull.

## Translation to Software

[[mary-poppendieck]] and [[tom-poppendieck]] translated pull production into software work management. The software equivalent of inventory is work-in-process: tasks started but not completed, features coded but not integrated, code merged but not deployed. Like manufacturing inventory, software WIP accumulates waste — it ties up attention, hides defects, and delays feedback.

A pull system for software means:

- Work is pulled into a stage only when that stage has capacity to process it (not pushed in based on a schedule).
- Work-in-process limits are set for each stage, preventing accumulation.
- Bottlenecks become visible as upstream stages stop pulling, allowing diagnosis and remediation.
- The pace of work is governed by actual throughput, not optimistic planning.

## Influence on David Anderson's Kanban Method

[[david-anderson]] developed the Kanban method for software and knowledge work in 2007, building directly on the Poppendiecks' lean software development work combined with his reading of [[donald-reinertsen]]'s queueing theory. Anderson's key innovations were:

1. **Explicit WIP limits** as the mechanism for implementing pull.
2. **Visualizing the workflow** on a kanban board, making WIP and bottlenecks visible.
3. **Flow metrics** (lead time, throughput, cycle time) as the primary measures of system performance.
4. **Evolutionary change** — starting with the existing process and improving incrementally rather than prescribing a new methodology.

The Poppendiecks had articulated the principle; Anderson operationalized it into a concrete method. The influence chain from [[taiichi-ohno]] to the Poppendiecks to Anderson is one of the clearest translation lineages in lean software development.

## Pull and the Delivery Pipeline

[[deliver-as-fast-as-possible]] is the principle that pull systems serve. Pull is the mechanism; fast delivery is the outcome. By limiting WIP and governing flow with pull signals, teams move work through the delivery pipeline faster and with fewer defects — because problems surface quickly and batches stay small.

[[value-stream-mapping-for-software]] is the tool for diagnosing where push behavior is creating WIP accumulation in the delivery pipeline, making it the diagnostic partner to pull system implementation.

## Relationship to DevOps

The pull-system logic extends naturally into the DevOps movement. [[gene-kim]]'s First Way of DevOps — Systems Thinking / Flow — is essentially pull production applied to the entire delivery pipeline from development through operations. Deployment pipelines, feature flags, and continuous delivery practices all implement pull: code is integrated and deployed when the downstream system is ready to receive it, not according to a quarterly release schedule that batches work independently of demand.
