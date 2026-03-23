---
id: donald-reinertsen
title: "Donald Reinertsen"
type: person
tags:
- product-development
- queueing-theory
- flow
- economics
links:
- target: principles-of-product-development-flow
  relation: related_to
  note: "Cross-KB expansion: Reinertsen's major work"
  kb: reinertsen
importance: 8
role: "Product development flow theorist"
affiliations:
- "Reinertsen & Associates"
research_status: draft
---

Donald Reinertsen is a product development theorist whose work on queueing theory, cost of delay, and batch size economics provided much of the quantitative backbone for the Poppendiecks' lean software development framework — particularly in [[implementing-lean-software-development-2006]].

## Queueing theory and flow

Reinertsen applied queueing theory to product development to show why high utilization rates produce disproportionately long cycle times. When a system operates near capacity, queues form and grow nonlinearly: a team at 80% utilization has dramatically shorter wait times than one at 95% utilization. This mathematical relationship underlies the Poppendiecks' arguments for slack, WIP limits, and avoiding the trap of optimizing for resource utilization rather than flow. [[deliver-as-fast-as-possible]] and [[optimize-the-whole]] both depend on this insight — local efficiency metrics (keeping every developer fully occupied) produce global inefficiency (slow throughput and long lead times).

## Cost of delay

Reinertsen's cost of delay framework makes the economic case for fast delivery explicit: delay has a real cost, and deferring decisions about when to deliver is not neutral. This connects directly to [[decide-as-late-as-possible]] — the Poppendiecks' principle is not about deferring decisions indefinitely but about not deciding prematurely, while still recognizing the cost that delay imposes on value delivery.

## Batch size economics

Reinertsen's analysis of how transaction costs and holding costs jointly determine optimal batch size gave the Poppendiecks a formal argument for small batches in software. When transaction costs (setup costs, deployment costs) are reduced, the optimal batch size shrinks. This is the economic logic behind continuous integration, frequent releases, and the elimination of inventory as one of the [[seven-wastes-of-software]].

## Relationship to the Poppendiecks

[[mary-poppendieck]] and [[tom-poppendieck]] draw on Reinertsen's work extensively throughout [[implementing-lean-software-development-2006]] and [[leading-lean-software-development-2009]]. His framing helped them move beyond analogy — "software is like manufacturing" — to principled argument: here is why the economics of flow apply to knowledge work, and here is the mathematics behind it. [[david-anderson]] similarly drew on Reinertsen when developing the Kanban method, making Reinertsen a shared intellectual source for both lean software and Kanban streams.
