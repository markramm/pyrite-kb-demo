---
id: acceptance-criteria
title: "Acceptance Criteria"
type: practice
importance: 5
tags:
- quality
- user-stories
- definition-of-done
- bdd
practice_type: quality
originated_in: "Agile / XP (complementary to user stories)"
status: active
research_status: draft
---

Acceptance criteria are the specific, testable conditions that must be satisfied for a [[user-stories|user story]] to be considered complete. They transform a story from a conversation placeholder ("As a user, I want to reset my password") into a testable specification ("Given a valid email address, when the user requests a password reset, then they receive a reset email within 60 seconds"). Acceptance criteria are distinct from but closely connected to the [[definition-of-done]] — the DoD applies to all stories; acceptance criteria are story-specific.

## Intellectual Contribution

Acceptance criteria solve a fundamental communication problem in Agile teams: user stories are intentionally brief and conversation-provoking, but they are too ambiguous to be tested. Acceptance criteria bridge the gap between a story's intent and its implementation without reverting to the heavyweight requirements documents that [[agile-manifesto-four-values]] reject in favor of [[responding-to-change]].

The practice reflects a key insight: requirements are not discovered once and then implemented — they are refined through conversation, and the acceptance criteria are the crystallized output of that conversation. This positions acceptance criteria as a learning artifact: the team's current best understanding of what "done" means for this story.

Well-written acceptance criteria follow the Given-When-Then format, borrowed from Behavior-Driven Development (BDD), a practice elaborated by Dan North from [[test-driven-development]]. BDD treats acceptance criteria as executable specifications: automated tests are written in Given-When-Then syntax and run against the implementation. This makes acceptance criteria not just communication tools but quality infrastructure — the automated acceptance test suite becomes the living specification.

## Relationship to Definition of Done

The [[definition-of-done]] is a team-level standard that applies to every story: code reviewed, unit tests passing, deployed to staging, etc. Acceptance criteria are story-specific: they define what this story must do, not how all stories must be built. A story can meet all acceptance criteria but fail the definition of done (e.g., criteria pass but code wasn't reviewed). Both are required for the story to be done.

## Connection to Sprint Review

At the [[sprint-review]], acceptance criteria provide the basis for the demonstration: the team shows each story's acceptance criteria being satisfied (or explains why they are not). This grounds the review in concrete, observable behavior rather than abstract progress claims.

Related practices: [[user-stories]], [[definition-of-done]], [[test-driven-development]], [[sprint-review]].
