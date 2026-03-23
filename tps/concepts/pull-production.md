---
id: pull-production
title: Pull Production
type: concept
tags:
- pull
- flow
- scheduling
- core-principle
links:
- target: pull-systems-in-software
  relation: influenced
  note: TPS pull production — producing only what downstream demand requires — is
    directly adapted by the Poppendiecks as pull systems for software development
  kb: poppendiecks
- target: flow-control
  relation: influenced
  note: TPS pull production and flow control are the manufacturing origin of Reinertsen's
    flow-based product development framework
  kb: reinertsen
importance: 8
first_appeared: Ohno's supermarket insight, late 1950s
related_concepts:
- kanban
- just-in-time
- one-piece-flow
- heijunka
research_status: draft
---

Production triggered by actual downstream demand rather than upstream forecasts or schedules. In push production (the mass-production default), a central plan schedules production at each station, pushing materials forward regardless of downstream need. In pull production, work begins only when a downstream process signals need — typically via [[kanban]]. [[taiichi-ohno]]'s insight came from the [[supermarket-visit-pull-production-insight|American supermarket]]: shelf space is replenished only when customers pull items from it. No demand, no production. Pull systems naturally limit work-in-progress, prevent overproduction (the worst of the [[seven-wastes-muda|seven wastes]]), and make actual demand visible throughout the system. The pull principle is TPS's most broadly applicable concept — it appears in Kanban for knowledge work (WIP limits), in DevOps (deployment triggered by readiness, not schedule), and in Agile (pulling stories from a backlog rather than assigning work to teams).
