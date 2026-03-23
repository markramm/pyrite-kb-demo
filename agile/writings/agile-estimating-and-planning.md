---
id: agile-estimating-and-planning
title: "Agile Estimating and Planning"
type: writing
importance: 7
tags:
- mike-cohn
- story-points
- velocity
- planning
- estimation
writing_type: book
date: 2005-11-01
author: "Mike Cohn"
publisher: "Prentice Hall"
research_status: draft
---

[[mike-cohn]]'s comprehensive treatment of estimation and planning in Agile contexts, published in 2005. The book codified [[story-points]] and [[velocity]] as planning tools, providing the quantitative infrastructure for Agile planning that [[user-stories-applied]] established qualitatively.

## Story points and velocity

[[story-points]] are a unitless measure of the size and complexity of a user story, estimated relative to other stories rather than in hours. [[mike-cohn]]'s book explains the cognitive basis for this: humans are better at relative estimation than absolute estimation. Estimating "this story is twice as big as that one" is more reliable than estimating "this story will take 14 hours."

[[velocity]] — the number of story points a team completes per iteration — is the empirical feedback mechanism. After a few iterations, a team's velocity stabilizes, providing a reliable basis for forecasting. This connects to [[empirical-process-control]]: instead of planning based on estimates made before work begins (which are unreliable), teams use measured [[velocity]] to forecast based on what they actually deliver.

The book covers:
- Why traditional estimation fails and the case for relative sizing
- Planning poker ([[planning-poker]]): the estimation technique using Fibonacci numbers
- Release planning: using velocity and story count to forecast release dates
- Iteration planning: selecting stories for each sprint
- Tracking and communicating: burndown charts, burnup charts

## Planning poker

[[planning-poker]] — team members simultaneously reveal estimate cards to avoid anchoring bias — is described in this book and became a widely adopted practice. [[mike-cohn]] formalized a practice that had been used informally in XP teams. The Fibonacci sequence (1, 2, 3, 5, 8, 13, 21...) used for cards reflects the increasing uncertainty in larger estimates.

## Influence

The book's treatment of story points and velocity became the de facto standard for Agile planning in [[scrum]] teams worldwide. Practices from this book are embedded in major Agile project tracking tools (Jira, Rally, VersionOne). The book also influenced release planning in [[safe-scaled-agile-framework]] and other scaling frameworks.

The approach has critics: story points are often misused as productivity metrics, gaming velocity becomes a problem, and some practitioners (including [[kent-beck]] himself) have questioned whether story points add more value than simpler counting approaches.

See also: [[user-stories-applied]] for the requirements companion to this planning book.
