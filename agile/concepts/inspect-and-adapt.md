---
id: inspect-and-adapt
title: "Inspect and Adapt"
type: concept
importance: 7
tags:
- feedback-loop
- scrum
- foundational
originator: "ken-schwaber"
concept_type: principle
research_status: draft
---

Inspect and adapt is the core Agile feedback loop: examine what is actually happening, then adjust based on what you find. The phrase is most strongly associated with [[scrum]] and [[empirical-process-control]], but the underlying pattern is present in every Agile method. [[kent-beck]]'s [[extreme-programming]] runs the loop through the test suite; [[alistair-cockburn]]'s [[crystal]] runs it through "reflection workshops"; the [[agile-manifesto-twelve-principles]] express it in principle 12 as regular retrospection and adjustment.

## Intellectual Roots

The inspect-and-adapt loop is a specific instance of a much older idea in control theory and organizational learning. W. Edwards Deming's Plan-Do-Check-Act (PDCA) cycle, later revised to Plan-Do-Study-Act (PDSA), is the most direct predecessor: plan an experiment, execute it, study the results, act on what you learned. Deming developed PDCA from Walter Shewhart's statistical process control work, which itself was rooted in the experimental method.

The pattern also appears in John Boyd's OODA loop (Observe-Orient-Decide-Act), which describes how effective decision-makers maintain tempo by cycling through observation and adaptation faster than their adversaries. [[responding-to-change]] — the fourth Agile value — is the strategic expression of the same logic: the team that can observe reality and adapt faster than the competition gains an advantage.

## Scrum's Implementation

[[ken-schwaber]] and [[jeff-sutherland]] built inspect-and-adapt into every level of Scrum's structure:

- **Daily**: The Daily Scrum inspects progress toward the Sprint Goal and adapts the day's plan.
- **Sprint**: The [[sprint-review]] inspects the Increment and adapts the Product Backlog. The [[retrospective]] inspects the team's process and adapts how they work.
- **Release**: The Product Backlog itself is a living artifact, continuously adapted as the Product Owner learns more about what creates value.

This multi-timescale structure distinguishes Scrum's implementation from simpler "check in occasionally" approaches. Inspection without adaptation is measurement theater; adaptation without inspection is arbitrary change. The pairing is what produces learning.

## Relationship to [[definition-of-done]]

Inspection requires a standard against which to inspect. The [[definition-of-done]] serves this function: it establishes what "done" means so that inspection of the Increment has a fixed reference point. Without it, inspection becomes subjective and adaptation is disconnected from reality. This connection — inspect-and-adapt requires transparency, and transparency requires shared definitions — is why the three pillars of [[empirical-process-control]] (transparency, inspection, adaptation) are named in that order.

## Beyond Scrum

The [[agile-manifesto-twelve-principles]]' principle 12 states the pattern without Scrum-specific language: "At regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behavior accordingly." The [[retrospective]] is the primary ceremony for this, and [[esther-derby]] (with Diana Larsen) systematized retrospective facilitation as a discipline. The [[heart-of-agile]]'s "Reflect" and "Improve" — two of [[alistair-cockburn]]'s four words — are direct descendants. The pattern is what survives when frameworks are stripped away.
