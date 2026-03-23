---
id: taiichi-ohno
title: "Taiichi Ohno"
type: person
importance: 8
tags:
- toyota
- tps
- lean-manufacturing
- waste
role: "Toyota Production System creator"
affiliations:
- "Toyota Motor Corporation"
relationship_to_poppendiecks: "Intellectual ancestor — created TPS that Poppendiecks translated to software"
research_status: draft
---

Taiichi Ohno was the chief engineer at Toyota who, working through the 1950s and 1960s, developed the operational system that would later be called the Toyota Production System (TPS). His foundational contribution was identifying waste — muda — as the central enemy of productive work, and building a production philosophy around its systematic elimination.

## The seven wastes

Ohno's seven wastes (overproduction, waiting, transportation, over-processing, inventory, motion, and defects) became the manufacturing baseline that [[mary-poppendieck]] and [[tom-poppendieck]] translated directly into [[seven-wastes-of-software]]. The translation was not a simple renaming: it required identifying what these structural failure modes looked like in a domain where the "product" is information and the "factory" is a software team. Partially done work, extra features, relearning, handoffs, task switching, defects, and waiting — the Poppendiecks' list — maps the logic of Ohno's categories onto software development reality.

## Just-in-time and pull

Ohno's just-in-time production principle — make only what is needed, when it is needed, in the amount needed — is the manufacturing source of [[deliver-as-fast-as-possible]] and [[pull-systems-in-software]]. Rather than push work downstream based on a schedule, pull production triggers upstream activity only when downstream demand exists. This structural logic underlies the Poppendiecks' treatment of flow and [[value-stream-mapping-for-software]].

## Kanban

Ohno invented the kanban card system to operationalize pull in Toyota's factories. This became the direct ancestor of [[david-anderson]]'s Kanban method for software teams, which extended the Poppendiecks' lean software thinking into an explicit visual management system.

## Jidoka

Ohno's second pillar of TPS — jidoka, or autonomation with a human touch — established the principle of stopping production when defects appear rather than passing them downstream. This is the manufacturing expression of [[build-integrity-in]]: quality is not inspected in at the end but designed into the process itself.

Ohno's ideas reached the Poppendiecks not only through [[james-womack]] and [[daniel-jones]]'s codification of lean for Western audiences but also through [[mary-poppendieck]]'s direct experience with lean manufacturing at [[3m-company]].
