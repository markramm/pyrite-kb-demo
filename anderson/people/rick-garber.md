---
id: rick-garber
title: "Rick Garber"
type: person
importance: 6
tags:
- corbis
- kanban-origins
- process-improvement
role: "Process improvement manager, Corbis"
relationship_to_subject: "Collaborator in designing the Corbis kanban implementation"
research_status: draft
---

Rick Garber managed the process improvement team at [[corbis]] when Anderson joined as Senior Director of Software Engineering in September 2006. The two collaborated on designing a kanban system intended to replace Corbis's dysfunctional project-centric approach to software delivery — a collaboration that produced the first fully articulated implementation of what would become the Kanban Method.

## The Corbis context

Corbis was a digital image licensing company owned by Bill Gates that had chronic delivery problems at the point Anderson arrived. The existing project management approach created long queues, unpredictable delivery, poor visibility into work status, and frequent escalations. Anderson and Garber worked together to diagnose the systemic causes of these problems and design a kanban-based system that would make workflow visible, limit WIP, and introduce explicit policies for handling different types of work.

## The design collaboration

Garber's process improvement background meant he could translate the theoretical framework Anderson brought — queueing theory, pull systems, WIP limits — into operational designs that the Corbis engineering teams could actually use. The Corbis implementation that emerged from this collaboration was more sophisticated than the [[microsoft-xit-kanban-2004]] experiment: it included explicit [[classes-of-service]] (the categorization of work items by cost-of-delay profiles), metrics for tracking lead time and throughput, and a workflow visualization (the kanban board) that showed not just current state but also policies. These features, developed in the Corbis environment with Garber's practical input, became the core practices documented in the [[kanban-book]].

## Relationship to later collaborators

Garber was the initial Corbis collaborator; [[corey-ladas]] and [[dan-vacanti]] joined the Corbis implementation later (winter 2007 and May 2007 respectively). The full [[corbis-kanban-experiment]] thus involved three collaborators at different stages, with Garber providing the foundational implementation work that Ladas and Vacanti then extended and refined.
