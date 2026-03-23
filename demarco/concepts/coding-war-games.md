---
id: coding-war-games
title: "Coding War Games"
type: concept
tags:
- empirical
- productivity
- research
- workplace-environment
links:
- target: common-cause-vs-special-cause-variation
  relation: related_to
  note: The Coding War Games found 10:1 productivity variation. Deming's framework distinguishes common-cause (system) from special-cause (individual) variation — DeMarco's finding is that workplace environment is a common cause, not individual talent
  kb: deming
importance: 9
metadata:
  first_appeared: "peopleware"
  key_writings: &id001
  - peopleware
  - why-does-software-cost-so-much
  related_concepts: &id002
  - peopleware-thesis
  - office-environment-effect
  - flow-and-interruption-cost
  - team-jell
  research_status: draft
first_appeared: "peopleware"
key_writings: *id001
related_concepts: *id002
research_status: draft
---

The Coding War Games is the empirical foundation of DeMarco and [[timothy-lister|Lister]]'s argument in [[peopleware]]. It was a multi-year productivity study conducted through the [[atlantic-systems-guild]] in which participants from different organizations completed the same standardized coding and testing exercise, allowing controlled comparison across hundreds of programmers and dozens of organizations.

## Study Design

The exercise was a defined programming task — participants implemented a specified program from scratch, then tested it against a battery of test cases. Participants were drawn from real software organizations: they completed the exercise individually, on their own time, using their own tools and environments. Their organizations' managers were asked to complete a companion survey about the workplace conditions — office size, noise levels, privacy, interruption frequency, and related factors.

This design was a significant methodological innovation. Rather than relying on self-reported productivity estimates or project-level metrics (which conflate individual contribution with team and project variables), the Coding War Games produced directly comparable performance data: time to complete, defect rate, and test passage rate.

## Key Findings

The most cited finding is a **10:1 variation** in individual productivity — the best performers completed the exercise in roughly one-tenth the time of the worst, with correspondingly lower defect rates. The magnitude of this variation had been noted by others (including [[fred-brooks]] and [[gerald-weinberg]]) but the Coding War Games provided unusually direct evidence.

Crucially, DeMarco and [[timothy-lister|Lister]] then asked: what predicts performance? Their analysis found that the standard candidates — years of experience, salary, programming language used, level of formal education — showed weak or negligible correlation with performance. What did correlate significantly was **workplace environment quality**, as reported by the companion organizational surveys.

The specific environmental factors that distinguished top performers included:

- More private, dedicated workspace
- Fewer reported interruptions during the workday
- Greater control over their physical environment (ability to quiet the space, close a door, reduce distractions)
- Less reported noise

This is the empirical anchor for the [[office-environment-effect]] argument and the [[flow-and-interruption-cost]] analysis.

## The Matched-Pair Analysis

One of the study's most compelling analytical moves was examining matched pairs: pairs of participants from the **same organization** who performed very differently. Within each pair, salary, experience, tools, and programming language are controlled — both people work in the same environment, use the same methods, and have similar backgrounds. Yet performance still varied substantially within pairs.

DeMarco and [[timothy-lister|Lister]] used this to argue against purely individual explanations. Even when you control for organizational context, individual variation remains significant — which is part of why they argue so strongly against interchangeable-parts thinking about programmers.

## Limitations and Context

The Coding War Games data comes from a standardized exercise rather than real project work, which means it may not fully capture the collaborative and architectural aspects of software development. The study also accumulated data over time across different administrations, which introduces methodological heterogeneity. DeMarco and [[timothy-lister|Lister]] acknowledge these limitations but argue the pattern is robust enough to be taken seriously.

The [[coding-war-games-study]] as a specific event refers to the ongoing data collection that fed the analysis in [[peopleware]] and subsequent work. The data continued to inform DeMarco and [[timothy-lister|Lister]]'s consulting and writing into the 1990s and beyond.

## Significance

The Coding War Games gave DeMarco and [[timothy-lister|Lister]] a rare commodity in software management writing: actual data. Most software management advice is based on anecdote, consulting experience, or reasoning from first principles. The ability to say "we measured this across hundreds of programmers" gave the [[peopleware-thesis]] a credibility that purely argumentative books lack.

The 10:1 productivity variation finding has become one of the most widely cited statistics in software engineering debates about individual differences, hiring, and workplace design — often cited without reference to its empirical source in the Coding War Games.
