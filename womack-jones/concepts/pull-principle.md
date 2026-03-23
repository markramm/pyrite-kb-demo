---
id: pull-principle
title: "Pull (Fourth Lean Principle)"
type: concept
importance: 8
tags:
- lean-thinking
- five-principles
- pull-system
- kanban
- demand-driven
first_appeared: "Lean Thinking (1996)"
key_writings:
- lean-thinking
- beyond-toyota
related_concepts:
- five-lean-principles
- flow-principle
- perfection-principle
- lean-production
tps_source: "TPS kanban system — the operational mechanism for demand-driven production, where downstream processes signal upstream processes to produce"
application_domain: general
research_status: draft
---

The fourth of the [[five-lean-principles]]: let the customer pull value from the producer. Instead of pushing products based on forecasts and production schedules, produce only what the next downstream step needs, when it needs it.

## The Principle

[[james-p-womack]] and [[daniel-t-jones]] position pull as the mechanism that connects production to actual demand. In [[lean-thinking]], they argue that once [[flow-principle|flow]] is established, the organization can let the customer's actual demand propagate backward through the value stream, triggering production only when needed. This eliminates the waste of overproduction — which [[taiichi-ohno]] considered the worst of the seven wastes because it generates all the others (inventory, waiting, transportation, etc.).

## TPS Source

Ohno's kanban system was the operational mechanism for pull at [[toyota-motor-corporation]]. A kanban (signal card) attached to a container of parts would be sent upstream when the downstream process consumed those parts, triggering production of exactly that quantity. The system was elegant in its simplicity: no central scheduling, no forecasting — just a physical signal propagating demand information backward through the production chain.

Womack and Jones abstract pull from kanban's physical mechanism to a general principle: design systems so that nothing is produced upstream until the customer downstream signals a need. This abstraction enables application to information products, services, and processes where physical kanban cards don't apply — but it also loses the specific disciplining mechanism that made pull work at Toyota. Without kanban's physical constraints, "pull" can become an aspiration rather than an operational reality.

## Relationship to Flow

Pull and [[flow-principle|flow]] are deeply interdependent in TPS. Flow makes pull possible (if work doesn't flow, pull signals can't propagate); pull disciplines flow (without demand signals, continuous flow produces overproduction). Womack and Jones present them as sequential steps 3 and 4, but in practice they must be implemented together. This is one of the points where the sequential framing of the [[five-lean-principles]] simplifies TPS's simultaneous, interlocking structure.

## Downstream Adoption

- Lean Startup's "validated learning" and minimum viable product concept are a form of pull: don't build features until customer demand is validated
- Agile software development's sprint backlogs and user-story prioritization are pull mechanisms
- Kanban boards in software (Trello, Jira) descend directly from Ohno's kanban through the lean transmission chain

## Research Needed

- How Womack/Jones's pull concept relates to Don Reinertsen's work on managing product development flow
- The specific case studies in Lean Thinking that illustrate pull implementation outside manufacturing
