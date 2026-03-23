---
id: kanban
title: Kanban
type: concept
tags:
- signaling
- pull
- production
- visual-management
links:
- target: wip-constraints
  relation: influenced
  note: TPS kanban cards are the physical instantiation of WIP constraints — Reinertsen
    abstracts this into a general queueing principle for product development
  kb: reinertsen
importance: 9
first_appeared: Introduced at Toyota's machine shop 1953; expanded across all plants by 1963
related_concepts:
- pull-production
- just-in-time
- one-piece-flow
- heijunka
research_status: draft
---

A visual signaling system for [[pull-production]] — physical cards (kanban literally means "signboard" or "visual card") that authorize production or movement of materials. When a downstream process consumes parts, the kanban card returns upstream, authorizing the production of replacement parts. No card, no production. [[taiichi-ohno]] was inspired by visiting American supermarkets in the 1950s: items on shelves are replenished only when customers pull them. The [[supermarket-visit-pull-production-insight|supermarket insight]] was one of TPS's founding moments. Kanban makes [[just-in-time]] operationally visible — inventory levels, production status, and bottlenecks are immediately apparent. The concept was later adapted for software development by David Anderson as "Kanban for knowledge work," where task cards on boards visualize workflow and limit work-in-progress (see [[tps-to-lean-software-transmission]]). Described in [[toyota-production-system-beyond-large-scale-production]] and [[workplace-management]].
