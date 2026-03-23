---
id: corbis-kanban-experiment
title: "Corbis Kanban Experiment (2006-2008)"
type: event
importance: 9
tags:
- kanban-method
- corbis
- classes-of-service
- wip-limits
- lead-time
date: 2006-09-01
location: "Seattle, WA"
participants:
- rick-garber
- corey-ladas
- dan-vacanti
status: confirmed
---

The Corbis Kanban Experiment refers to Anderson's design and evolution of a kanban system at [[corbis]] between September 2006 and his departure in 2008 — the sustained empirical work that produced the Kanban Method in its mature form. Anderson arrived at Corbis as Senior Director of Software Engineering with a theoretical framework from [[don-reinertsen]]'s queueing theory and an experimental template from the [[microsoft-xit-kanban-2004]] event; Corbis was the laboratory in which that framework was tested, refined, and extended into a comprehensive change management method.

## The starting point

When Anderson joined Corbis in September 2006, the software engineering organization used a project-centric delivery model that was failing: projects ran late, costs were unpredictable, and the queue of requested work was poorly managed. Anderson and [[rick-garber]] (process improvement manager) began designing a kanban system as a replacement, drawing on the virtual pull system model from the Microsoft experiment but extending it to the more complex demands of a digital asset management and licensing business.

## The key developments

By March 2007 — six months into the Corbis engagement and after [[corey-ladas]] joined as process coach in winter 2007 — the kanban system had evolved to include the practices that would define the mature Kanban Method:

**Workflow visualization**: The kanban board made the entire workflow visible, from initial request through acceptance to delivery. Work items were represented as cards (physical or virtual) on a board showing their current stage, assigned team, and status. The visual transparency was itself a management tool: it surfaced bottlenecks, revealed WIP accumulation, and made policies visible to everyone.

**WIP limits** ([[wip-limits]]): Each stage of the workflow had an explicit limit on the number of work items that could be present simultaneously. When a stage reached its limit, upstream stages could not push more work in — creating the pull dynamic that distinguished the system from a push-based project schedule.

**Classes of service** ([[classes-of-service]]): Work items were categorized by their cost-of-delay profiles into four classes: expedite (urgent, high cost of further delay), fixed-date (deadline-driven), standard (normal flow), and intangible (improvement work with no direct revenue impact). Each class had different WIP allocations and scheduling policies. This was a direct application of [[don-reinertsen]]'s cost-of-delay framing to the scheduling problem of heterogeneous knowledge work.

**Lead time metrics**: The system tracked how long each work item took from commitment to delivery, generating a distribution that could be analyzed with statistical process control techniques. The lead time data enabled evidence-based conversations about delivery predictability and identified systemic issues contributing to long or variable lead times.

**Operations reviews**: Regular management meetings were restructured around flow metrics — lead time distributions, throughput, WIP levels, and classes-of-service mix — rather than project status reports. This changed the management conversation from "what is the status of Project X?" to "how is the system performing and what is constraining it?"

[[dan-vacanti]] joined as ERP project development manager in May 2007, bringing additional rigor to the metrics side of the implementation.

## The 2007 presentation

The [[corbis-kanban-presentation]] — Anderson's presentation of the Corbis work at Reinertsen's 2007 LSSC (Lean Software and Systems Consortium) conference — was the first public presentation of the method. It introduced classes of service and lead time analysis to the broader product development community and established the intellectual connection between the empirical Corbis case study and Reinertsen's queueing theory framework.

## Significance

The Corbis experiment is the foundational empirical case for the Kanban Method. It is where the six core practices were established through empirical observation rather than theoretical derivation, where the key metrics (lead time, throughput, WIP) were validated as practical management tools, and where the evolutionary change thesis — start with what you do now, introduce pull, improve from there — was tested in a live organizational context. The [[kanban-book]] is substantially a documentation of what was learned at Corbis.
