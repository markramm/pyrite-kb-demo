---
id: less-large-scale-scrum
title: "LeSS (Large-Scale Scrum)"
type: concept
importance: 5
tags:
- scaling
- scrum
- larman
originator: "craig-larman"
concept_type: framework
research_status: draft
---

Large-Scale Scrum (LeSS) is a scaling framework created by Craig Larman and Bas Vodde, first described in their books "Scaling Lean & Agile Development" (2008) and "Practices for Scaling Lean & Agile Development" (2010), and later in "Large-Scale Scrum" (2016). LeSS positions itself as a principled extension of [[scrum]] to multi-team contexts rather than a new framework, and its guiding principle — "more with LeSS" — encodes its philosophy: descale the organization rather than add framework layers.

## The Core Argument

LeSS is built on a critique of how organizations typically respond to coordination problems at scale. When multiple teams need to coordinate, the conventional response is to add layers: program managers, release trains, portfolio processes. LeSS argues this is exactly backwards. The coordination overhead is a symptom of organizational dysfunctions — too many hand-offs, siloed component teams, separated "business" from "technical" — not a natural feature of scale. The solution is to fix the dysfunctions rather than manage around them.

This is a more structurally radical position than [[safe-scaled-agile-framework]]. SAFe accepts the large organization as given and adds coordination mechanisms. LeSS prescribes organizational changes — cross-component feature teams, reduced product ownership layers, merged backlogs — that reduce the coordination problem at its source.

## Basic LeSS

For 2-8 teams (up to ~50 people):

- One Product Backlog, one Product Owner, one overall product definition
- Each team runs a standard Scrum Sprint
- A single Sprint Review for all teams together
- Teams share a Definition of Done ([[definition-of-done]])
- Overall Retrospective plus team retrospectives ([[inspect-and-adapt]])
- No additional coordination roles (no Release Train Engineer, no Program Manager)

## LeSS Huge

For 8+ teams: introduces Area Product Owners (responsible for a subset of the product, not a separate layer) and Requirement Areas (customer-facing partitions of the backlog). LeSS Huge avoids creating a "meta-PO" layer by keeping Area Product Owners subordinate to the overall Product Owner.

## The Organizational Change Requirement

LeSS's primary weakness in enterprise adoption is identical to its primary intellectual strength: it requires real organizational change, not just framework adoption. Implementing LeSS means eliminating project manager roles, restructuring component teams into feature teams, and removing management layers. These changes are politically difficult and organizationally disruptive. [[safe-scaled-agile-framework]] can often be adopted by adding roles without eliminating existing ones; LeSS cannot.

This makes LeSS more faithful to [[agile-manifesto-four-values]] — particularly [[self-organizing-teams]] and [[responding-to-change]] — but less accessible to organizations whose leadership is unwilling to change power structures. In Larman's own framework practice, he has documented that organizational resistance to feature teams is the single most common failure mode of LeSS adoption.

## Relationship to Scrum

LeSS is explicitly positioned as [[scrum]] scaled, not a new framework. The [[scrum-guide]] remains the foundation; LeSS adds only what is necessary for multi-team coordination. This fidelity to Scrum is both principled — Larman and Vodde believe Scrum's simplicity is a feature, not a limitation — and a direct critique of SAFe's complexity.
