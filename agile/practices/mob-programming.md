---
id: mob-programming
title: "Mob Programming"
type: practice
importance: 5
tags:
- collaboration
- woody-zuill
- ensemble
- whole-team
practice_type: collaboration
originated_in: "Practitioner innovation (Woody Zuill, c. 2012)"
status: active
research_status: draft
---

Mob programming — recently rebranded "ensemble programming" — is the practice of having the whole team work together on one thing, at one computer, at the same time. A single developer (the "driver") types; the rest of the team (the "mob" or "navigators") directs what the driver types, contributes ideas, spots problems, and manages context. Roles rotate on a timer (typically every 10–15 minutes). Woody Zuill and his team at Hunter Industries discovered and named the practice around 2012, and Zuill became its primary champion through talks and his book "Mob Programming: A Whole Team Approach" (2017, with Kevin Meadows).

## Intellectual Contribution

Mob programming extends [[pair-programming]]'s logic to its limit. Where pairing addresses the problem of solo work's isolation, mobbing eliminates isolation entirely — all decisions are made collaboratively, all code is reviewed in real time, all knowledge is immediately shared. The intellectual claim is not that mob programming is always optimal but that its costs are lower and its benefits higher than conventional wisdom suggests.

The benefits Zuill and practitioners report are significant: defect rates drop dramatically (real-time review is more thorough than code review), integration problems disappear (everyone is integrated in the same work), onboarding is accelerated (new developers learn from the whole team continuously), and [[technical-debt]] accumulates more slowly (no one can cut corners without the mob noticing).

The practice also makes [[collective-code-ownership]] genuinely rather than nominally true: when the whole team builds everything together, knowledge of the codebase is uniformly distributed by construction. This eliminates the bus-factor problem that [[pair-programming]] only mitigates.

## Connection to Agile Principles

Mob programming embodies [[individuals-and-interactions]] in its most radical form. It also operationalizes [[sustainable-pace]] differently than expected: practitioners report that mobbing is less mentally exhausting than expected because cognitive load is shared. The social dynamic of the mob maintains focus in ways that solo work does not.

The practice connects to [[self-organizing-teams]]: mobs are self-directing by structure — there is no project manager directing traffic when the whole team is in the room together.

## Current Status

Mob programming remains a niche practice — far less common than [[pair-programming]]. It faces organizational resistance based on the intuition (often stated by management) that having five people do one person's work must be wasteful. Practitioners counter that the quality and coordination benefits outweigh the apparent waste, but the evidence base remains limited to practitioner reports and case studies rather than controlled studies.
