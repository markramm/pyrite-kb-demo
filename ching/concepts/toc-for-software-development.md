---
id: toc-for-software-development
title: "TOC for Software Development"
type: concept
importance: 10
tags:
- toc
- software-development
- agile
- constraint
- throughput
goldratt_source: "Theory of Constraints (general)"
application_domain: software-development
first_appeared: "early career, ~2003"
research_status: draft
---

TOC for Software Development is Ching's overarching framework — the synthesis that defines his entire intellectual project. It holds that [[eliyahu-goldratt]]'s Theory of Constraints, originally developed for factory-floor throughput, applies directly to software delivery, but requires translation because the nature of constraints in knowledge work is fundamentally different from manufacturing.

## The Core Insight

In a factory, bottlenecks are visible: work-in-progress piles up in front of a slow machine. The constraint is physical, observable, and stable for reasonable periods. In software development, constraints are largely invisible:

- **Skill constraints** — specialized expertise held by one or two people (the senior architect, the lone DBA, the QA lead who knows the legacy system)
- **Decision constraints** — work stalled waiting for approval, sign-off, or a product owner who is overcommitted
- **Testing capacity** — a manual QA process that can't absorb the throughput of a fast development team
- **Environment constraints** — shared test environments that become a choke point across multiple teams
- **Integration constraints** — downstream systems or third parties that can't accept deliveries at the pace of development

Because these constraints don't produce visible queues of physical goods, they go unrecognized — and improvement effort gets directed elsewhere, producing no throughput gain.

## The Agile-TOC Synthesis

Ching discovered TOC around 2003 and encountered Agile methods in roughly the same period. His central argument is that the two frameworks are natural complements rather than competitors:

- **Agile** provides the iterative delivery framework: short cycles, fast feedback, working software over documentation
- **TOC** provides the analytical framework: where is the actual constraint on delivery, and how do we exploit it?

Without TOC, Agile teams often speed up development while the bottleneck sits elsewhere — testing, deployment, stakeholder review. They produce more WIP without increasing throughput. Without Agile, TOC practitioners in software lack the iterative structure needed to act on what the constraint analysis reveals.

[[gene-kim]]'s "The Phoenix Project" (2013) independently demonstrated TOC thinking applied to software and DevOps, using the Three Ways as a parallel formulation. Ching had been developing similar ideas in his consulting work and in [[rolling-rocks-downhill]]. The convergence validates the framework from a different angle.

[[david-anderson]]'s Kanban work and [[steve-tendon]]'s TameFlow approach represent adjacent efforts to apply flow thinking to software — Ching's contribution is positioned as more accessible and more explicitly narrative in its pedagogy.

## Development Arc

This synthesis is the throughline of Ching's career across the [[early-career-and-toc-discovery]], [[writing-and-consulting-period]], and [[bottleneck-guy-brand-period]] eras. It grounds [[rolling-rocks-downhill]], [[the-bottleneck-rules]], and [[the-bottleneck-detective]], and is what distinguishes [[oddsocks-consulting]]'s approach from generic Agile coaching. The [[focccus-formula]] is the most compressed expression of this framework in practice.
