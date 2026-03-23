---
id: working-software
title: "Working Software"
type: concept
importance: 7
tags:
- manifesto
- values
- delivery
originator: "agile-manifesto-signatories"
concept_type: principle
research_status: draft
---

"Working software is the primary measure of progress" — principle 7 of the [[agile-manifesto-twelve-principles]] — and "Working software over comprehensive documentation" — value 2 of the [[agile-manifesto-four-values]] — together constitute the decisive break Agile made with document-driven development. The concept appears at both the values level (what matters more) and the principles level (how you measure it), giving it unusual structural weight in the manifesto.

## The Problem It Named

By the late 1990s, large enterprise software projects had developed an elaborate infrastructure of documentation that served as a proxy for progress. Requirements specifications, design documents, review sign-offs, test plans — each gate produced paper artifacts that could be audited and reported to management. The actual software was often a distant output, appearing late and frequently failing to do what the specifications promised. The specifications had been reviewed and approved; the software did not match what users needed; both facts were simultaneously true.

The working software principle is a direct attack on this proxy-progress economy. If the only legitimate measure of progress is software that actually works — that executes, that users can interact with, that meets acceptance criteria — then document production cannot be claimed as progress. This was culturally radical: it invalidated large portions of what project management offices, auditors, and waterfall methodologists measured.

## What "Working" Means

The precision matters. "Working" in the Agile sense means meets the [[definition-of-done]]: it executes, passes its tests, meets the team's quality standards, and is potentially shippable. Not "works in development," not "compiles," not "passes the demo with known bugs." The [[scrum-guide]]'s concept of the "Increment" formalizes this: each Sprint produces an increment of working software that meets the Definition of Done and is potentially releasable.

[[test-driven-development]] is the technical practice most directly aligned with this principle: the test defines what "working" means before the code is written. [[continuous-integration]] ensures that "working" is validated continuously rather than discovered at the end.

## Working Software and Documentation

The qualifier in the value — "while there is value in the items on the right" — has been routinely dropped in popularizations of Agile. The manifesto does not prohibit documentation. It asserts a priority when the two conflict. In [[dark-agile]] implementations, this has been used to justify refusing all documentation; in [[agile-industrial-complex]] contexts, it has been used to sell process frameworks that generate new forms of documentation (PI Plans, SAFe Program Backlogs) while nominally honoring the value.

[[martin-fowler]] and others have argued that certain types of documentation — particularly documentation of architectural decisions and APIs — actually support agility by making code more maintainable. The productive reading of the value is: documentation should serve the software, not substitute for it.

## Lineage

The emphasis on working software has a lean manufacturing parallel: in lean, value is defined by what the customer experiences, not by what internal metrics track. A product moving through production is not value until it reaches the customer. Similarly, a document describing software is not value until the software exists and works. This alignment between the working software principle and lean's value-stream thinking was one of the intellectual connections the Poppendiecks developed in their lean software development work.
