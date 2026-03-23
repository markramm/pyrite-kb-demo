---
id: scrum
title: "Scrum"
type: concept
importance: 10
tags:
- framework
- scrum
- empirical
originator: "ken-schwaber"
concept_type: framework
research_status: draft
---

Scrum is the dominant Agile framework by market share and organizational adoption. Created by [[ken-schwaber]] and [[jeff-sutherland]], it operationalizes [[empirical-process-control]] through a small set of roles, events, and artifacts. Its power is its deliberate incompleteness: Scrum defines the boundaries of an empirical process but leaves the interior — how the team actually builds software — intentionally unspecified. This makes it lightweight enough to adopt widely, but also creates the conditions for [[dark-agile]] implementations that adopt the ceremonies without the underlying values.

## Origins

[[jeff-sutherland]] traces Scrum's origins to [[hirotaka-takeuchi]] and [[ikujiro-nonaka]]'s [[new-new-product-development-game]] (1986), which used the "scrum" rugby metaphor to describe self-organizing product development teams at Japanese manufacturers. Sutherland's first Scrum implementation was at Easel Corporation in 1993; [[ken-schwaber]] was developing similar ideas independently. They presented the framework together at [[oopsla-scrum-presentation-1995]] in 1995, and Schwaber published [[agile-software-development-with-scrum]] in 2002. The [[scrum-guide]], first published in 2010 and substantially revised in 2020, is the canonical definition.

## Structure

**Roles (as of the 2020 [[scrum-guide]]):**
- **Product Owner** — maximizes value, owns and orders the Product Backlog, represents stakeholder needs
- **Scrum Master** — accountable for Scrum being understood and enacted; servant-leader and coach
- **Developers** (previously "Development Team") — the people doing the work of building the Increment

**Events:**
- **Sprint** — the container for all other events; fixed duration (≤4 weeks); produces a releasable Increment
- **[[sprint-planning]]** — establishes the Sprint Goal and the Sprint Backlog
- **Daily Scrum** — 15-minute inspection of progress toward the Sprint Goal (not a status report to a manager)
- **[[sprint-review]]** — inspects the Increment, adapts the Product Backlog
- **[[retrospective]]** — inspects the team's process, identifies improvements

**Artifacts:**
- **Product Backlog** — ordered list of everything needed for the product; owned by the Product Owner
- **Sprint Backlog** — the Sprint Goal plus the plan for delivering it
- **Increment** — the sum of completed Product Backlog Items meeting the [[definition-of-done]]

## The [[scrum-alliance]] and Institutionalization

[[ken-schwaber]], [[mike-cohn]], and [[esther-derby]] co-founded the [[scrum-alliance]] in 2002, establishing the Certified ScrumMaster (CSM) certification that became the movement's highest-volume credential. Schwaber left the Scrum Alliance in 2009 ([[schwaber-leaves-scrum-alliance-2009]]) to found [[scrum-org]], creating competing certification tracks and a division in Scrum's institutional identity.

## Why Scrum Won the Framework War

Scrum's dominance over [[extreme-programming]] in enterprise adoption reflects several factors: its organizational focus (rather than XP's technical focus) made it more accessible to managers; its certification program created commercial infrastructure; its role structure (Product Owner, Scrum Master) created new career paths. Critics — including [[ron-jeffries]], XP's co-creator — have argued that Scrum's technical agnosticism allowed adoption without the engineering practices (like [[test-driven-development]] and [[continuous-integration]]) that make rapid iteration sustainable, producing what Jeffries called "Dark Scrum."
