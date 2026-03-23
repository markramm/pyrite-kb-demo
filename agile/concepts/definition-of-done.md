---
id: definition-of-done
title: "Definition of Done"
type: concept
importance: 6
tags:
- scrum
- quality
- transparency
originator: "scrum-community"
concept_type: practice
research_status: draft
---

The Definition of Done (DoD) is a shared team commitment specifying the conditions that must be met before a product increment can be considered complete. It is the [[scrum]] community's formalization of an answer to a question that plagued software projects: "done" meant different things to different people, and that disagreement accumulated as invisible [[technical-debt]] until it became a delivery crisis.

## Why It Exists

Before the Definition of Done became standard Agile practice, "done" was negotiated informally, often at the moment of inspection. A developer would say a feature was done; a tester would find defects; the developer would argue the defects were in a different part of the system; the product manager would accept the feature as "done enough" under schedule pressure. The result was a body of software that was nominally complete but carried undisclosed quality deficiencies.

The Definition of Done makes this negotiation explicit, in advance, and binding. It is a quality standard that the team collectively maintains, not a bar set by management. In [[scrum]]'s framework, the DoD is what makes [[empirical-process-control]] possible: transparency requires that "done" means the same thing to everyone, inspection requires a standard to inspect against, and adaptation requires honest data about what has and hasn't been completed.

## What a Definition of Done Typically Includes

Common elements, which vary by context and maturity:

- Code is written and peer-reviewed
- Unit tests written and passing
- Integration tests passing
- [[continuous-integration]] build passing
- Code meets [[acceptance-criteria]] (from the story)
- Documentation updated where relevant
- Performance meets specified thresholds
- Security review completed (for relevant stories)
- No new [[technical-debt]] introduced without explicit tracking

More mature teams may include: deployed to staging, product owner acceptance, accessibility criteria met.

## The [[scrum-guide]] Formalization

The 2017 and 2020 [[scrum-guide]] revisions elevated the Definition of Done to a formal Scrum artifact (rather than just a practice) and clarified that it applies to the Increment, not just individual backlog items. The 2020 Guide explicitly states that if a Product Backlog item does not meet the Definition of Done, it cannot be included in the Sprint Review — the DoD is a hard gate, not a guideline.

The Guide also introduced the concept of organizational DoD: if the organization has a definition of done that is broader than any single team's, teams must meet the organizational standard as a minimum and may extend it. This formalization was partly a response to [[dark-agile]] patterns in which teams maintained separate definitions of done for "development done" and "release done," hiding significant undone work.

## Relationship to [[inspect-and-adapt]]

The Definition of Done is infrastructure for [[inspect-and-adapt]]. Without it, the Sprint Review inspects against an undefined standard — different stakeholders bring different expectations, and the feedback produced is not calibrated. With it, the Sprint Review has a shared baseline: did the Increment meet the Definition of Done? Is the Definition of Done itself adequate for the product's needs? The second question makes the Definition of Done itself subject to [[inspect-and-adapt]] — it should evolve as the team's capability and the product's requirements evolve.
