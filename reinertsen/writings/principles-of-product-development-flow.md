---
id: principles-of-product-development-flow
title: "The Principles of Product Development Flow: Second Generation Lean Product Development"
type: writing
importance: 10
tags:
- product-development
- queueing-theory
- lean
- economics
- flow
writing_type: book
date: "2009-01-01"
coauthors: []
key_concepts:
- cost-of-delay
- queueing-theory-applied
- batch-size-reduction
- wip-constraints
- u-curve-optimization
- decentralized-control
- weighted-shortest-job-first
- economic-framework-for-prioritization
- cadence-and-synchronization
- fast-feedback
- managing-variability
- flow-control
research_status: draft
---

Reinertsen's magnum opus and definitive theoretical statement. The book organizes 175 principles across eight thematic areas: economics, queueing, variability, batch size, [[wip-constraints|WIP constraints]], [[flow-control]], sequencing, and [[decentralized-control]]. Together these constitute what Reinertsen calls "second generation" lean product development.

The "second generation" label carries a pointed critique. First-generation lean product development — as practiced by many agile and lean software advocates in the 2000s — mechanically transplanted manufacturing lean tools without understanding the underlying economics. Reinertsen's argument is that lean works in manufacturing for specific reasons tied to the economics of physical production, and that transplanting the tools without the economic reasoning produces cargo-cult lean: practices that look right but fail in different contexts. The second generation must be grounded in economics and queueing mathematics, not tool adoption.

The book's treatment of [[cost-of-delay]] is its most influential contribution. Reinertsen argues that [[economic-framework-for-prioritization|sequencing decisions]] should be made by comparing the cost of delay per unit of time against the duration of the work item — the ratio now called [[weighted-shortest-job-first]] (WSJF). This framework was directly adopted by [[dean-leffingwell]] in SAFe and [[scaled-agile-inc]], making it one of the most widely deployed prioritization methods in large-scale agile.

The book's treatment of variability is particularly distinctive. Where manufacturing lean treats variability as pure waste to be eliminated, Reinertsen argues that variability in product development is sometimes valuable because it generates information — the uncertain experiment that fails teaches something. The goal is therefore [[managing-variability|managing variability]], not eliminating it, a distinction with significant implications for how development processes should be designed.

The [[queueing-theory-applied|queueing theory]] material draws on [[john-little|Little's Law]] and related results to explain why high utilization rates destroy flow, why large batches create queues, and why [[cadence-and-synchronization|cadence and synchronization]] improve predictability. [[david-anderson]] cites this work as a direct foundation for Kanban in software development, particularly the use of [[wip-constraints]] to control queue length and cycle time.

The book opens with a diagnostic framework: the [[twelve-cardinal-sins]] of product development — twelve common failures (from failure to quantify economics to centralized control) that the 175 principles address. It also introduces the [[batch-size-death-spiral]], a reinforcing feedback loop where large batches attract additional scope and overhead, making batches ever larger. [[eric-ries]] called the book "quite simply the most advanced product development book you can buy," and it directly shaped his Build-Measure-Learn framework in "The Lean Startup." [[mik-kersten]]'s Flow Framework for software delivery likewise builds explicitly on this work.

The relationship to [[managing-the-design-factory]] is one of synthesis and extension: the earlier book introduced the key concepts; this one provides the comprehensive theoretical framework, the mathematical grounding, and the 175-principle structure that makes it a reference work as much as a linear argument. Published by [[celeritas-publishing]], Reinertsen's own imprint, it has been translated and used in his "Second Generation Lean Product Development" seminars worldwide. The book inaugurates the [[flow-synthesis-period]] era, and its publication is documented in the event [[publication-principles-of-flow]].
