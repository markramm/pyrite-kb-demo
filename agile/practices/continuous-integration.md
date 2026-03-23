---
id: continuous-integration
title: "Continuous Integration"
type: practice
importance: 8
tags:
- technical
- xp
- automation
- martin-fowler
practice_type: technical
originated_in: "Extreme Programming (XP)"
status: active
research_status: draft
---

Continuous Integration (CI) is the practice of integrating every developer's work into the shared mainline frequently — at least daily, ideally after every small change — and verifying each integration with an automated build and test suite. It originated in [[extreme-programming]] and became the technical foundation on which modern DevOps pipelines rest.

[[martin-fowler]] wrote the definitive article on CI (2006, updated 2024 on martinfowler.com), establishing the canonical rules: maintain a single source repository, automate the build, make the build self-testing, every commit triggers a build, fix broken builds immediately, keep the build fast, test in a production-like environment. These rules encode a discipline, not just a tool configuration.

## Intellectual Contribution

CI's central insight is that integration problems — the painful merging of divergent code branches — compound with time. Long-lived branches accumulate difference; integration is painful in proportion to that difference. CI eliminates the accumulation by making integration continuous. This reframes integration from a phase (something done at the end of development) to a practice (something done constantly, at low cost per occurrence).

This logic connects directly to [[agile-manifesto-twelve-principles]]: "Deliver working software frequently." CI is the technical mechanism that makes frequent delivery feasible. Without an automated build-and-test pipeline, frequent integration would be prohibitively expensive.

## Relationship to Other Practices

CI requires [[test-driven-development]] to be meaningful — a build that doesn't run tests catches compilation errors but not behavioral regressions. It enables [[collective-code-ownership]] by providing a safety net: any developer can change any code and immediately know whether they've broken something. And it is the foundation of continuous delivery and deployment, which extended CI's logic to production releases.

[[working-software]] as the primary measure of progress is meaningless without a mechanism to verify that software is working continuously. CI operationalizes this principle. The practice also embodies [[inspect-and-adapt]]: each integration is a feedback loop, surfacing problems at the smallest possible unit.

## Current Status

CI is now infrastructure rather than practice — major platforms (GitHub Actions, GitLab CI, Jenkins, CircleCI) make automated pipelines the default. The original intellectual contribution has been absorbed so thoroughly that its radical nature in 2001 is easy to forget: the norm in pre-Agile shops was integration events separated by weeks or months.
