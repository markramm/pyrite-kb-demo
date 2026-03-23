---
id: story-points
title: "Story Points"
type: practice
importance: 6
tags:
- planning
- estimation
- mike-cohn
- velocity
- noestimates
practice_type: planning
originated_in: "XP / Agile estimation (popularized by Mike Cohn)"
status: contested
research_status: draft
---

Story points are abstract, relative units of effort used to estimate the size of [[user-stories]] and backlog items. Rather than estimating in hours or days, teams assign points on a relative scale (commonly Fibonacci: 1, 2, 3, 5, 8, 13...) by comparing stories to each other: "this story is about twice as complex as that one, so if that one is a 3, this one is a 5." Over time, a team's average throughput in points per sprint stabilizes as [[velocity]], which is then used to forecast future delivery.

[[mike-cohn]] is the primary popularizer of story points through [[agile-estimating-and-planning]] (2005) and [[succeeding-with-agile]], though the technique was circulating in XP communities before he formalized it.

## Intellectual Contribution

Story points' core intellectual claim is that relative estimation is more reliable than absolute estimation. Humans are demonstrably poor at judging absolute durations ("this will take four days") but reasonably good at comparative judgments ("this is about twice as complex as that"). Story points exploit this asymmetry: by anchoring estimates to a reference story and reasoning comparatively, teams may produce more calibrated forecasts than with hour-based estimates.

A secondary claim is that decoupling estimate from time removes pressure to inflate or deflate estimates for political reasons. When story points carry no direct conversion to person-hours, estimates are somewhat insulated from schedule negotiation dynamics.

Story points combine with [[velocity]] to create a planning instrument: if a team consistently delivers 30 points per sprint, and the remaining backlog contains 300 points, the team can forecast approximately 10 more sprints to completion. This is the mechanism [[sprint-planning]] uses for longer-horizon forecasting.

## Controversy: The NoEstimates Movement

Story points are the most contested practice in the Agile canon. Critics make several arguments: (1) velocity is self-fulfilling — teams tend to fill the sprint and then adjust estimates backward to make velocity constant; (2) story point inflation is endemic — as teams are pressured to deliver more, story sizes creep upward; (3) the relative calibration degrades as team composition, technology, and problem domain shift; (4) the entire estimation activity is waste — flow metrics (cycle time, throughput measured in stories or features) provide better forecasting data with less overhead.

[[ron-jeffries]], one of TDD's originators, has publicly questioned the value of story points. [[kent-beck]] has expressed skepticism about velocity gaming. The NoEstimates movement (Vasco Duarte, Neil Killick, Woody Zuill) argues for flow-based planning without size estimation.

## Current Status

Story points remain dominant in Scrum-practicing organizations, institutionalized through certification curricula and tooling (Jira defaults). The controversy is genuine and unresolved.

Related practices: [[planning-poker]], [[sprint-planning]], [[velocity]], [[user-stories]].
