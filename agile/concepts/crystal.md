---
id: crystal
title: "Crystal"
type: concept
importance: 6
tags:
- methodology
- cockburn
- people-centered
originator: "alistair-cockburn"
concept_type: methodology
research_status: draft
---

Crystal is a family of software development methodologies created by [[alistair-cockburn]], distinguished by being calibrated to project size and criticality rather than prescribing a single approach. The core insight is that methodology should be a function of what a project requires, not a universal prescription. Crystal is arguably the lightest-weight of the pre-manifesto methods and the one most explicitly grounded in empirical research about what software teams actually do.

## The Color System

Crystal methodologies are named by color, with weight increasing as the names progress:

- **Crystal Clear** — for teams of 2-8 people working on non-life-critical software. Described in [[crystal-clear]] (2004).
- **Crystal Yellow** — for teams of 10-20 people
- **Crystal Orange** — for teams of 20-50 people
- **Crystal Red** — for teams of 50-100 people
- Darker colors (Maroon, Diamond) for larger or higher-criticality projects

The calibration is explicit: a 6-person team developing internal business software needs far less process than a 40-person team building medical device software. Universal methodology prescriptions ignore this variation and impose overhead that serves no purpose at the small end or insufficient rigor at the high-criticality end.

## Core Values

Crystal's emphasis is captured in seven properties, with the first three considered most essential:

1. **Frequent delivery** — shipping working software to real users regularly, even if not continuously
2. **Reflective improvement** — teams regularly reflect on their process and adjust ([[inspect-and-adapt]])
3. **Osmotic communication** — team members absorb project information through proximity; this is the empirical basis for co-location preferences

Additional properties include personal safety (ability to raise concerns without punishment — what later became "psychological safety"), focus, easy access to expert users, and automated tests.

## Cockburn's Empirical Approach

Unlike [[scrum]] and [[extreme-programming]], which were developed from first principles and conviction, Crystal emerged from [[alistair-cockburn]]'s empirical study of software projects in the early 1990s. He interviewed and observed teams at IBM and elsewhere to understand what actually characterized successful projects. The finding was consistently human-centered: project success correlated with communication quality, team cohesion, and individual skill more than with process compliance.

This empirical grounding gives Crystal a different character. Where XP says "do TDD," Crystal says "ensure your team has feedback mechanisms that work for your size and criticality — here are some options." The flexibility is principled, not permissive.

## Crystal at Snowbird and After

[[alistair-cockburn]] brought Crystal to [[snowbird-meeting-2001]] as one of the represented methodologies. His participation shaped the manifesto's emphasis on communication and people over process. After Snowbird, Crystal remained less widely adopted than [[scrum]] or [[extreme-programming]] in enterprise contexts — partly because its deliberate flexibility made it harder to certify and sell as a product. Cockburn's later [[heart-of-agile]] initiative can be read as a distillation of Crystal's core to its essence: Collaborate, Deliver, Reflect, Improve.
