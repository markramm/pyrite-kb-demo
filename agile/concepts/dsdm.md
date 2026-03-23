---
id: dsdm
title: "DSDM (Dynamic Systems Development Method)"
type: concept
importance: 6
tags:
- methodology
- uk
- rad
originator: "dsdm-consortium"
concept_type: methodology
research_status: draft
---

Dynamic Systems Development Method (DSDM) is a project delivery framework founded by the [[dsdm-consortium]] in the United Kingdom in 1994. It emerged from the Rapid Application Development (RAD) tradition pioneered by James Martin and institutionalized it through an industry consortium that gave it governance, training infrastructure, and a formal body of knowledge. [[arie-van-bennekum]] represented DSDM at [[snowbird-meeting-2001]] and signed the [[agile-manifesto]].

## Origins in RAD

DSDM grew from practitioners' experience with RAD in the early 1990s. RAD had demonstrated that software could be delivered faster by prioritizing working prototypes over comprehensive specifications and by involving users throughout the development process. The problem was that RAD lacked a formal framework — it was more an attitude than a methodology. The DSDM Consortium, formed by seventeen founding organizations in 1994, codified RAD principles into a repeatable framework that could be trained, audited, and certified.

The consortium model was significant: DSDM was owned by its member organizations, not a single vendor, which gave it a different governance character than vendor-driven methodologies. The [[dsdm-consortium]] became a genuine industry body.

## Eight Principles

DSDM's principles (the current DSDM Agile Framework version):

1. **Focus on the business need** — all decisions serve the business objective
2. **Deliver on time** — timebox as the primary mechanism; fix time and vary scope ([[iron-triangle]])
3. **Collaborate** — teams including business and technical people work together
4. **Never compromise quality** — the [[definition-of-done]] equivalent: agreed quality standards are not traded against time
5. **Build incrementally from firm foundations** — understand the domain before committing architecture
6. **Develop iteratively** — acknowledge that understanding evolves through building
7. **Communicate continuously and clearly** — formal documentation is supplemented by face-to-face
8. **Demonstrate control** — make the process visible and auditable

## Timeboxing as DSDM's Core Contribution

DSDM's most significant technical contribution to the Agile movement is the formalization of **timeboxing**: fixing the duration of a development period and varying scope to fit, rather than fixing scope and letting time slip. This directly inverts the conventional project management assumption and is the mechanism through which [[responding-to-change]] becomes operationally possible. The fixed-time box creates a forcing function: what is most valuable must be done first, and less valuable scope is deferred rather than used to justify schedule extension.

Timeboxing in DSDM predates the Scrum Sprint by roughly a year, though both were emerging simultaneously in different contexts. The Sprint and the DSDM timebox are independent convergences on the same solution to the same problem.

## MoSCoW Prioritization

DSDM formalized the MoSCoW method for scope management within timeboxes: **M**ust have, **S**hould have, **C**ould have, **W**on't have (this time). The technique acknowledges that not all scope is equal and makes the prioritization conversation explicit. It has spread far beyond the DSDM community into general project management.

## Legacy and Current Status

DSDM has remained primarily a UK and European phenomenon and is less widely known in the US market. The DSDM Consortium has continued to evolve the framework (now marketed as "DSDM Agile Framework" or "AgilePM") and to position it as an enterprise governance-compatible alternative to Scrum. Its emphasis on business case justification and auditability has made it attractive in government and regulated-industry contexts where Scrum's informality is a barrier.
