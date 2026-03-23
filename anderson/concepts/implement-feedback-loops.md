---
id: implement-feedback-loops
title: "Implement Feedback Loops"
type: concept
importance: 7
tags:
- core
- cadences
- review
- adaptation
- meetings
first_appeared: "kanban-book"
key_writings:
- kanban-book
- essential-kanban-condensed
- kanban-maturity-model
related_concepts:
- kanban-method
- make-policies-explicit
- improve-collaboratively
- evolutionary-change
- manage-flow
- kanban-maturity-model-concept
source_tradition: "Deming (PDSA cycle), original"
research_status: draft
---

Implement Feedback Loops is the fifth of the six core practices of Anderson's [[kanban-method]]: establishing regular cadences at which participants review the system's performance and adapt its policies and design.

## The Seven Feedback Loops

The mature Kanban Method defines seven specific feedback loops (developed in [[kanban-book]] and elaborated in subsequent training materials):

1. **Daily Standup** — team-level coordination, focused on blocked items and flow impediments (not status reports). The question is "what is blocking flow?" not "what did you do yesterday?"
2. **Replenishment Meeting** — team and upstream stakeholders review the backlog, select items to commit to, and pull work into the system. Typically weekly or bi-weekly.
3. **Kanban Meeting / Queue Replenishment** — a shorter tactical meeting focused on which items to pull into active work from the committed queue.
4. **Delivery Planning Meeting** — coordinates delivery of completed work to downstream customers or operations.
5. **Service Delivery Review** — a periodic (typically monthly) review of the service's performance: lead times, throughput, quality, [[fitness-criteria]] against customer expectations.
6. **Operations Review** — a management-level review across multiple services or teams, examining portfolio-level flow and identifying systemic issues.
7. **Strategy Review** — a higher-frequency strategic review examining whether the services being offered remain appropriate for the business context.

The seven loops are not all required from day one. The [[evolutionary-change]] principle applies: teams implement the cadences that address their most pressing needs, then add others as the system matures.

## Why Cadences Matter

Anderson drew on systems thinking (and implicitly on [[w-edwards-deming]]'s PDSA cycle) to argue that improvement requires regular, structured opportunities for reflection. Without established cadences, review happens ad hoc — usually only when something goes wrong, and usually in a blame-oriented mode. Regular feedback loops create a normalized, constructive context for examining performance.

The cadence structure also serves a political function: it provides regular, scheduled access to stakeholders and management in a format designed for information sharing rather than escalation. The Service Delivery Review and Operations Review loops are explicitly designed to give management visibility into service performance without requiring constant interruption of the delivery team.

## Feedback Loops and [[classes-of-service]]

The Replenishment Meeting is where [[classes-of-service]] decisions are made: work items are categorized by risk and urgency profile as part of the commitment decision. The Service Delivery Review examines whether the SLAs associated with each class of service are being met. The feedback loops operationalize the class-of-service framework at the process level.

## Relationship to Scrum's Ceremonies

Anderson explicitly distinguished Kanban's feedback loops from Scrum's ceremonies. Scrum mandates sprint planning, daily standup, sprint review, and retrospective at fixed intervals determined by the sprint length. Kanban's feedback loops are:

- Not tied to iteration boundaries (Kanban doesn't use iterations)
- Not all required — the team implements what is needed
- Scaled in frequency to their purpose (daily standups are daily; strategy reviews may be quarterly)
- Designed around flow metrics and service performance rather than iteration deliverables

This distinction was significant in the Kanban-vs-Scrum debates: Anderson was not arguing that Kanban teams never meet, but that meeting cadences should be appropriate to the system's needs, not mandated by an iteration calendar.

## Maturity Progression

The [[kanban-maturity-model-concept]] maps feedback loop sophistication to organizational maturity levels. Early-maturity organizations typically have only a daily standup and an informal replenishment process. Higher-maturity organizations have all seven loops operating with defined participants, formats, and escalation paths. The Operations Review and Strategy Review loops are particularly associated with enterprise Kanban: they represent the scaling of the method beyond individual teams to portfolio and organizational levels.
