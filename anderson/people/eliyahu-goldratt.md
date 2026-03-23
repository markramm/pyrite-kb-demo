---
id: eliyahu-goldratt
title: "Eliyahu Goldratt"
type: person
importance: 7
tags:
- theory-of-constraints
- systems-thinking
- bottlenecks
- throughput
role: "Physicist, management theorist, creator of Theory of Constraints"
relationship_to_subject: "Intellectual source; TOC was the framework for Anderson's first book and influenced the initial kanban implementations"
research_status: draft
---

Eliyahu Goldratt (1947–2011) was an Israeli physicist who became one of the most influential management theorists of the late twentieth century. His Theory of Constraints (TOC) — introduced to a wide audience through the business novel "The Goal" (1984) and systematized in "The Theory of Constraints" (1990) and "Critical Chain" (1997) — provided Anderson with the foundational framework for his early work in agile software management and influenced the first kanban implementations at [[microsoft]].

## Theory of Constraints

TOC's central insight is that in any system, one constraint (bottleneck) limits overall throughput, and that improvement efforts directed at non-constraints are largely wasted. Goldratt's Five Focusing Steps — identify the constraint, exploit it, subordinate everything else to it, elevate it, and repeat — provided a systematic method for continuous improvement centered on throughput rather than local efficiency. The associated concepts of throughput (the rate of generating money through sales), inventory (all money invested in things the system intends to sell), and operating expense gave managers a three-variable economic lens sharply different from traditional cost accounting.

## Anderson's first book

[[agile-management-for-software-engineering]] (2003), Anderson's first major book, explicitly applied TOC to software engineering. It used Goldratt's throughput-accounting framework to challenge the cost-accounting logic that typically drives software project management, and proposed that software teams should be managed for throughput — finishing and delivering work — rather than for local resource utilization. This TOC orientation shaped Anderson's thinking about pull systems, bottlenecks, and the relationship between WIP and throughput before he encountered [[don-reinertsen]]'s queueing theory framework.

## Drum-Buffer-Rope and the Microsoft experiment

Goldratt's Drum-Buffer-Rope (DBR) scheduling mechanism — in which the constraint (drum) sets the production pace, a buffer protects the constraint from starvation, and a rope limits WIP upstream — was the direct inspiration for Anderson's first kanban-like system at [[microsoft]] in the [[microsoft-xit-kanban-2004]] event. Anderson designed that system as a DBR implementation for software support work, with the constraint (the offshore development team in India) setting the pace and WIP limited by the buffer size. It was only after conversations with [[don-reinertsen]] in winter 2005 that Anderson reframed this experiment in terms of virtual kanban systems and queueing theory.

## Position relative to Reinertsen

In Anderson's intellectual biography, Goldratt represents the first theoretical lens through which he analyzed knowledge work flow, while Reinertsen represents the more rigorous and ultimately more influential second framework. The Kanban Method's concern with throughput, bottlenecks, and pull systems reflects the TOC influence; its specific mechanisms (WIP limits quantified by queueing theory, cost-of-delay framing of [[classes-of-service]]) reflect the deeper Reinertsen influence. The two frameworks are largely compatible, and the [[kanban-book]] draws on both without treating them as alternatives.
