---
id: goldratt-to-software-transmission-chain
title: "The Goldratt-to-Software Transmission Chain"
type: note
importance: 7
tags:
- toc
- software
- transmission
- goldratt-descendant
- intellectual-history
---

Theory of Constraints originated in Israeli manufacturing in the late 1970s and early 1980s. By the mid-2010s, versions of it had become foundational to the DevOps movement, the Kanban Method, and multiple approaches to Agile software development. This note traces the paths that carried TOC from its manufacturing origins to software practice, and locates Ching's contribution within that transmission.

## The source: Goldratt's TOC

[[eliyahu-goldratt]] developed TOC through his scheduling software company and then through a series of business novels — "The Goal" (1984), "It's Not Luck" (1994), "Critical Chain" (1997), "Isn't It Obvious?" (2009). The core insight is simple and powerful: every system has one binding constraint; improvement efforts that do not address the constraint are waste; identify the constraint, exploit it, subordinate everything else to it, and only then invest in elevating it. The Five Focusing Steps formalize this cycle.

Goldratt's manufacturing context was a feature, not a bug: the clarity of physical constraints in a factory made the logic legible. A machine that can only process 100 units per hour is visibly the constraint when downstream capacity is 200. Software doesn't have machines. The question each of Goldratt's intellectual descendants answered differently was: what is the constraint in a software delivery system?

## Four transmission paths

**Goldratt → Ching → Agile+TOC for software project management**

Ching encountered Goldratt's work around 2003 and spent the following decade developing the translation. His answer to the software constraint question: the constraint in most software projects is decision-making capacity, specialist knowledge (often a single person who understands the system), or the integration and testing process. [[rolling-rocks-downhill]] dramatizes this through a software crisis scenario; [[the-bottleneck-rules]] distills it into the [[focccus-formula]]. Ching's transmission is the most narrative-driven of the four paths — he follows Goldratt's own pedagogical method of teaching through fiction. His reach is smaller than Kim's but his fidelity to the Goldratt tradition is higher.

**Goldratt → Gene Kim → The Phoenix Project → DevOps movement**

[[gene-kim]] co-authored "The Phoenix Project" (2013), a direct structural descendant of "The Goal" applied to IT operations. Kim's "Three Ways" — flow, feedback, continual learning — are a translation of TOC's systemic flow thinking into DevOps terms. The Phoenix Project reached a massive audience through the DevOps movement and became the foundational text of a major industry shift. Kim subsequently co-authored "The DevOps Handbook" and "Accelerate," extending the reach further. Goldratt's influence on DevOps runs almost entirely through Kim; the transmission was validated at scale.

**Goldratt → David Anderson → Kanban Method**

[[david-anderson]] drew on TOC, Lean, and systems thinking to develop the Kanban Method — a specific workflow management system for knowledge work with WIP limits, visual boards, and pull scheduling. Anderson's answer to the software constraint question was: the constraint is wherever work piles up; use WIP limits to make it visible and manage it. The Kanban Method is the most systematic and methodologically explicit of the four translations. Anderson published "Kanban: Successful Evolutionary Change for Your Technology Business" in 2010.

**Goldratt → Steve Tendon → TameFlow**

[[steve-tendon]] created TameFlow, combining TOC with Agile and Csikszentmihalyi's psychological flow state concept. TameFlow addresses both the systemic constraint question (where is work bottlenecking?) and the cognitive question (are people in a state that enables high performance?). It is the most theoretically ambitious translation, integrating a psychological layer that neither Goldratt nor the other transmitters developed. Tendon published "Hyper-Productive Knowledge Work Performance" (2015).

## What the paths share

All four paths share the core Goldratt insight: identify and manage the constraint; stop optimizing non-constraints. All four reject the naive response to delivery problems ("hire more people," "work faster," "add process") in favor of systemic diagnosis. And all four found narrative or accessible formats — business novels, podcasts, visual frameworks — rather than academic texts.

## What distinguishes them

- **Reach**: Kim's path reached the largest audience by far, through the DevOps movement and corporate IT adoption.
- **Fidelity to pedagogy**: Ching's path is the most faithful to Goldratt's own narrative teaching method.
- **Methodological rigor**: Anderson's path is the most systematically developed as a specific workflow methodology.
- **Theoretical integration**: Tendon's path is the most ambitious in integrating complementary frameworks.

## The contrast: the Deming transmission

The parallel Deming→Toyota→Lean→Agile transmission traveled through a different manufacturing tradition. Deming's System of Profound Knowledge, Toyota's Production System, Lean manufacturing, and then Lean software development represent a distinct intellectual lineage from Goldratt's TOC. Both lineages arrived at similar recommendations — reduce WIP, manage flow, identify waste/constraints, empower workers — through different theoretical routes.

The Goldratt transmission is more constraint-focused and more comfortable with narrative pedagogy; the Deming-Toyota transmission is more statistical, more concerned with variation reduction, and more rooted in the Toyota organizational model. Ching's work sits clearly in the Goldratt lineage; [[david-anderson]]'s Kanban Method draws from both traditions.

## Ching's specific contribution

Within the Goldratt-to-software transmission chain, Ching's distinctive contribution is accessibility and narrative fidelity. He reaches practitioners who would not read a management textbook, uses stories to make systemic thinking intuitive, and maintains the Goldratt tradition of the Socratic mentor figure. He is not the highest-reach transmitter (that is Kim) nor the most methodologically rigorous (that is Anderson), but he is the most direct inheritor of Goldratt's own teaching style — and the only one who has preserved a direct recorded conversation with Goldratt himself in [[six-lessons-with-eli-goldratt]].
