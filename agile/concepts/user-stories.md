---
id: user-stories
title: "User Stories"
type: concept
importance: 7
tags:
- requirements
- xp
- cohn
originator: "kent-beck"
concept_type: practice
research_status: draft
---

User stories are a requirements format expressing what a user wants from a system and why: "As a [type of user], I want [some goal] so that [some reason]." The format originated in [[extreme-programming]] as [[kent-beck]]'s "story cards" — index cards on which customers wrote what they wanted the system to do, which developers then estimated and which customers prioritized. [[mike-cohn]] systematized and popularized the format in [[user-stories-applied]] (2004), which remains the definitive reference.

## From Story Cards to User Stories

In [[xp-explained-first-edition]], Beck described "story cards" as the unit of the planning game: the customer writes a feature they want; the developer estimates how long it will take; the customer decides whether to include it in the current release based on cost and priority. The cards were physical objects on a wall — an early [[information-radiators|information radiator]].

The "As a... I want... so that..." structure was not in Beck's original formulation — it emerged from the XP community's practice and was formalized by [[mike-cohn]]. The structure does several things: it names a user type (forcing consideration of who benefits), specifies a goal (in user terms, not technical terms), and requires a reason (the benefit, which is the real requirement). The reason clause is the most commonly omitted; its absence often indicates that the story is a feature specification rather than a genuine user need.

## Stories and [[acceptance-criteria]]

A user story without acceptance criteria is incomplete. Acceptance criteria define the conditions that must be true for the story to be considered done — they bridge between the story (what the user wants) and the [[definition-of-done]] (what the team's quality standards require). The combination — story + acceptance criteria — replaces both the traditional requirements specification and the test plan for a feature: the story describes the desired behavior; the acceptance criteria define how you know it's there.

[[test-driven-development]] extends this: acceptance criteria can drive acceptance tests, which drive unit tests. BDD (Behavior-Driven Development), an extension of TDD, formalizes this connection using Given/When/Then syntax that is explicitly derived from story acceptance criteria.

## The INVEST Criteria

[[mike-cohn]] popularized the INVEST acronym as a checklist for well-formed stories:
- **I**ndependent — can be developed without depending on other stories
- **N**egotiable — the story is a conversation starter, not a contract
- **V**aluable — delivers value to a user or customer
- **E**stimable — the team can estimate its size
- **S**mall — fits in a single Sprint or iteration
- **T**estable — has clear acceptance criteria

Stories that fail INVEST criteria are candidates for splitting, clarification, or rejection.

## Relationship to the Product Backlog

In [[scrum]], user stories became the dominant format for Product Backlog items, though the [[scrum-guide]] does not require this format. The alignment is natural: stories are user-centered (connecting to the Product Owner's responsibility to maximize value), estimable (enabling [[sprint-planning]] and [[velocity]] tracking), and small enough to complete within a Sprint. The story format also facilitates the backlog refinement conversation between Product Owner and developers.

## Critique

User stories have been criticized for being over-applied. Not every backlog item is appropriately expressed as a user story: technical tasks, infrastructure work, and research spikes do not always have users who want something. Forcing technical work into story format can produce awkward constructions that obscure rather than clarify. [[mike-cohn]] has acknowledged this — stories are appropriate for user-facing features; other formats are appropriate for other work.
