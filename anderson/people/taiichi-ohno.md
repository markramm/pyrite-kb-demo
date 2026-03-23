---
id: taiichi-ohno
title: "Taiichi Ohno"
type: person
importance: 7
tags:
- toyota-production-system
- kanban
- lean
- pull-systems
- just-in-time
role: "Industrial engineer, creator of Toyota Production System"
relationship_to_subject: "Originator of the kanban concept that Anderson adapted for knowledge work"
research_status: draft
---

Taiichi Ohno (1912–1990) was a Japanese industrial engineer who served as executive vice president of Toyota and who designed the Toyota Production System (TPS) — the manufacturing philosophy that gave rise to the global Lean movement. His most famous publication, "Toyota Production System: Beyond Large-Scale Production" (1978, English translation 1988), is the primary source for understanding the kanban system in its original manufacturing context.

## The original kanban system

Ohno's kanban system was a production scheduling tool for physical manufacturing. Kanban cards (Japanese: signboard or card) authorized the movement of materials and the production of parts between workstations. When a downstream process consumed a part, it returned the kanban card to the upstream process, authorizing production of a replacement. This pull mechanism — production triggered by actual downstream consumption rather than by forecasts or production schedules — was the key innovation that allowed Toyota to minimize inventory, expose quality problems immediately, and synchronize production across complex assembly lines. The kanban system was one component of the broader TPS, which also included just-in-time delivery, jidoka (automation with a human touch), and a comprehensive approach to waste elimination (muda).

## The adaptation challenge

Anderson's relationship to Ohno is one of creative adaptation across a fundamental domain discontinuity. Ohno's system was designed for physical manufacturing, where inventory is tangible, WIP limits can be enforced by physical space and card counts, and the connection between a card and a specific physical part is direct. Knowledge work — software development, design, analysis — lacks physical inventory, and work items do not flow through a production line in the same sense. Anderson's contribution was to show that a virtual kanban system — a WIP-limited pull mechanism without physical cards, implemented in software like Microsoft Product Studio — could serve as a change mechanism for knowledge work even when the original manufacturing rationale did not translate directly.

## What Anderson took and what he transformed

From Ohno, Anderson took the core concepts of pull systems, visual management of work-in-progress, and the insight that making WIP visible and limiting it creates pressure to resolve systemic problems. What Anderson substantially transformed was the purpose: where Ohno's kanban system was primarily a production scheduling tool aimed at inventory reduction and quality, Anderson's Kanban Method was primarily a change management approach aimed at evolutionary organizational improvement. The [[kanban-book]] is explicit about this distinction — Anderson is not proposing that software teams use kanban cards in the Toyota sense, but that the discipline of WIP limits and visual workflow management can serve as a Trojan horse for organizational change.

## The naming question

The use of the word "kanban" to describe Anderson's method has occasionally caused confusion, since practitioners familiar with TPS sometimes expect a direct functional equivalence that does not exist. Anderson has addressed this by distinguishing Toyota's kanban system (a replenishment scheduling tool) from the Kanban Method (a change management approach) — a distinction that the [[kanban-book]] maintains throughout and that the KB guidelines identify as one of the three layers of "kanban" that must not be conflated.
