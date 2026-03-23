---
id: continuous-integration
title: "Continuous Integration"
type: practice
importance: 8
tags:
- delivery
- automation
- xp-origins
- dora-predictor
- trunk-based
practice_type: delivery
originated_in: "Kent Beck's Extreme Programming (1999); evolved through CI servers (CruiseControl, Hudson/Jenkins)"
evidence_base: "DORA/Accelerate: trunk-based development with CI is a strong predictor of software delivery performance"
related_practices:
- trunk-based-development
- deployment-automation
- version-control-everything
status: active
research_status: draft
---

Continuous Integration (CI) is the practice of merging all developers' working copies to a shared mainline frequently — at least daily, ideally after every commit. The core discipline: every integration is verified by an automated build-and-test sequence. If the build breaks, fixing it is the team's top priority. Code that cannot be integrated continuously cannot be shipped continuously.

## Origins: XP and the Integration Problem

CI emerged from Kent Beck's Extreme Programming in the late 1990s as a direct response to "integration hell" — the experience, common in waterfall and early Agile projects, of developers working in isolation for weeks or months and then spending painful weeks merging their divergent codebases. XP's response was radical: integrate constantly so that divergence never accumulates.

The XP practice required a shared codebase and a fast, automated test suite. Without tests, you cannot know whether an integration broke anything. Without automation, integration is too slow to do continuously. CI thus bundles together three disciplines: shared mainline development ([[trunk-based-development]]), test automation, and build automation.

## Tooling Evolution

CI became practically accessible through tooling:

- **CruiseControl** (2001, ThoughtWorks): the first open-source CI server. Polled the version control system, ran builds automatically on change, reported results.
- **Hudson** (2004, Sun Microsystems / Kohsuke Kawaguchi): significantly easier to configure; became the dominant CI server.
- **Jenkins** (2011): Hudson forked after Oracle acquired Sun. Jenkins became the standard for self-hosted CI throughout the 2010s.
- **Cloud CI** (Travis CI 2011, CircleCI 2011, GitLab CI 2012): CI as a service, eliminating the need to maintain CI infrastructure. Made CI accessible to open-source projects and smaller teams.
- **GitHub Actions** (2019): CI integrated directly into the version control host, further reducing friction.

The tooling evolution tracks the broader DevOps principle that automation should eliminate friction from the delivery path.

## Connection to the First Way

CI is a core First Way practice (see [[three-ways]]). The First Way demands fast flow of work through the value stream. Long-lived feature branches are waste: they delay integration, accumulate merge risk, and slow the feedback loop between development and testing. CI enforces small batch sizes — every commit is a batch — and makes the current state of integration visible at all times.

The [[deployment-pipeline]] extends CI downstream: CI handles the build-and-test phase; the pipeline extends that automation through staging environments to production. CI is the entry point to the pipeline.

## DORA Evidence

[[accelerate-book]] (Forsgren, Humble, Kim; 2018) identifies CI as a technical practice associated with high software delivery performance. Specifically, the [[state-of-devops-report-series]] shows that high performers practice [[trunk-based-development]] with CI — not long-lived branches with infrequent integration. The causal mechanism is clear: CI reduces batch size and integration risk, which enables faster flow and more frequent deployment.

[[dora-four-key-metrics]]: CI directly affects Deployment Frequency and Lead Time for Changes — the two flow metrics. Teams that cannot integrate continuously cannot deploy frequently.

## Common Failure Modes

CI fails when treated as a tool rather than a discipline:

- **Broken builds left unrepaired**: if the team tolerates a red build for days, CI provides no benefit. The discipline is "fix it immediately or revert."
- **Slow test suites**: if the CI build takes 45 minutes, developers batch their commits to avoid waiting. This recreates the integration delay CI was meant to eliminate. Fast feedback requires fast tests.
- **Branching strategies that defeat CI**: long-lived feature branches mean code is not actually being integrated continuously, regardless of whether a CI server exists. CI and [[trunk-based-development]] are inseparable.

## Relationship to Continuous Delivery

CI is the first stage of [[continuous-delivery]]: you cannot deliver continuously if you cannot integrate continuously. CI ensures the codebase is always in a state that could in principle be deployed. CD extends that assurance through automated testing in production-like environments and [[deployment-automation]]. The CI/CD abbreviation bundles the two practices, but they are conceptually distinct: CI is about integration; CD is about delivery readiness.
