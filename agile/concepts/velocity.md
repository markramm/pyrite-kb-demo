---
id: velocity
title: "Velocity"
type: concept
importance: 6
tags:
- planning
- measurement
- story-points
originator: "xp-community"
concept_type: pattern
research_status: draft
---

Velocity is a team's rate of work, measured in [[story-points]] (or other relative units) completed per iteration. It is used for forecasting: if a team completes 30 points per Sprint, a backlog of 150 points implies approximately 5 Sprints of work remaining. [[mike-cohn]] developed the most systematic treatment of velocity in [[agile-estimating-and-planning]] (2005). The concept is widely adopted and widely misused — its weaponization as a performance metric is among the most frequently cited [[dark-agile]] pathologies.

## What Velocity Is For

Velocity is a forecasting tool, not a performance metric. Its intended use is to answer the question: "Given what we know about this team's rate of work on this codebase, how long will it take to deliver this backlog?" A stable velocity makes forecasting more reliable; an unstable velocity signals something worth investigating (process changes, team changes, estimation drift).

The key structural property: velocity is team-specific, codebase-specific, and context-specific. A team that completes 30 points per Sprint is not "slower" or "faster" than a team that completes 50 points per Sprint — they are using different scales for their [[story-points]], working in different codebases, or operating under different constraints. [[story-points]] are not universal units; they are relative units calibrated to a specific team's reference stories.

## The Weaponization Problem

The most common and most damaging misuse of velocity is using it as a performance metric: "Team A does 40 points per Sprint; Team B does 30 points. Team B must improve their velocity." This use violates the concept's fundamental properties:

1. Teams will inflate estimates to hit velocity targets (story point inflation), making forecasts progressively less reliable
2. Teams will cut quality corners to complete more items (increasing [[technical-debt]])
3. Teams will stop collaborating on difficult problems (individual gaming of the metric)
4. [[sustainable-pace]] is abandoned as teams sprint to hit velocity targets

[[ron-jeffries]] and [[kent-beck]] have both written that using velocity as a management target is a reliable way to destroy both the usefulness of velocity as a tool and the team dynamics that produce good work. This is a specific instance of Goodhart's Law: a measure that becomes a target ceases to be a good measure.

## Velocity and [[planning-poker]]

The estimation process that produces story points typically uses [[planning-poker]], a group technique that prevents anchoring and surfaces disagreement. The quality of velocity as a forecasting tool depends on the quality of the estimation process: if [[planning-poker]] conversations are genuine — surfacing different mental models and producing calibrated estimates — velocity will be meaningful. If they are rushed or performative, velocity is noise.

## Yesterday's Weather

[[mike-cohn]] popularized the "yesterday's weather" principle: the best predictor of how much a team will complete next Sprint is how much they completed last Sprint. The principle is deliberately modest: it rejects the waterfall ambition of deriving throughput from resource calculations and replaces it with direct empirical observation. This is [[empirical-process-control]] applied to planning.
