---
id: software-project-rescue
title: "Software Project Rescue"
type: concept
importance: 7
tags:
- software-development
- project-management
- toc
- constraint
- agile
goldratt_source: "Five Focusing Steps applied to project management"
application_domain: software-development
first_appeared: "Rolling Rocks Downhill (2014)"
research_status: draft
---

Software project rescue is the specific applied context around which Ching built his consulting practice and his signature novel [[rolling-rocks-downhill]]. It describes the use of TOC to turn around late or failing software projects — not by adding resources or cutting scope, but by identifying and relieving the constraint that is actually preventing delivery.

## The Scenario

The canonical project rescue scenario in Ching's work involves a compressed deadline that cannot be moved, a scope that cannot be meaningfully cut without destroying the project's purpose, and a team that is already working hard. The question is not "how do we add capacity" but "what is actually stopping us from delivering, and how do we fix that specific thing?"

[[rolling-rocks-downhill]] is structured entirely around this scenario: Steve (Flora) must deliver a software project in far less time than anyone thinks is possible. The novel follows her applying TOC thinking — guided by a Goldratt-inspired mentor — to find the actual constraint and subordinate everything to it.

## Why Generic Project Management Fails

Standard project management responses to a failing project tend to:
- Add developers (which often slows delivery in the short term due to onboarding and coordination costs — Brooks's Law)
- Cut features (which may not address the constraint if the constraint isn't feature-development capacity)
- Extend the deadline (not available in rescue scenarios)
- Increase pressure (which raises stress without improving throughput)

Ching's TOC-based approach is different because it is constraint-focused rather than resource-focused or schedule-focused. The question is always: what single thing is most limiting throughput right now? Improving anything else is, in Goldratt's terms, an illusion of improvement.

## Connection to Critical Chain

[[eliyahu-goldratt]]'s Critical Chain Project Management (CCPM) is the formal TOC application to project scheduling, introduced in Goldratt's novel "Critical Chain" (1997). Ching draws from both CCPM and the general Five Focusing Steps / [[focccus-formula]] — his work is not a strict CCPM implementation but uses CCPM's core insight that project buffers should protect the whole project rather than individual tasks.

## The Rescue Moves

The diagnostic and intervention pattern in Ching's work:

1. **Find** — identify what is actually constraining delivery (see [[constraint-identification-in-knowledge-work]])
2. **Stop doing what doesn't serve the constraint** — work that doesn't feed the bottleneck is waste in a rescue situation
3. **Protect the constraint's time** — ensure the bottleneck is never starved of work or blocked by dependencies
4. **Buffer strategically** — put time buffers where they protect delivery, not distributed across every task

This applies [[toc-for-software-development]] in its most time-pressured, highest-stakes form, and it is the scenario that gave Ching his consulting brand at [[oddsocks-consulting]] and established him as a practitioner in [[agile-scotland]] circles.
