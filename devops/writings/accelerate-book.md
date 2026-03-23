---
id: accelerate-book
title: "Accelerate: The Science of Lean Software and DevOps: Building and Scaling High Performing Technology Organizations"
type: writing
importance: 10
tags:
- empirical-research
- dora-metrics
- software-delivery-performance
- foundational-text
writing_type: book
date: 2018-03-27
author: nicole-forsgren
coauthors:
- Jez Humble
- Gene Kim
publisher: "IT Revolution Press"
key_concepts:
- dora-four-key-metrics
- software-delivery-performance
research_status: draft
---

The empirical validation of the DevOps movement. Won the Shingo Publication Award. Based on four years of the DORA (DevOps Research and Assessment) [[state-of-devops-report-series]], encompassing more than 23,000 survey responses from technology professionals worldwide.

[[nicole-forsgren]] (organizational psychologist and researcher), [[jez-humble]], and [[gene-kim]] synthesized the research findings into a book that did something no prior DevOps text had done: proved with survey-based causal analysis that DevOps practices measurably improve organizational performance.

## The DORA Four Key Metrics

The book identified four metrics that distinguish high-performing software delivery organizations from low performers:

1. **Deployment Frequency** — how often code is deployed to production
2. **Lead Time for Changes** — time from commit to production deployment
3. **Change Failure Rate** — percentage of deployments causing production failures
4. **Time to Restore Service** — time to recover from production failures

These became the [[dora-four-key-metrics]] framework, now widely adopted as the standard measures of software delivery performance.

## The Central Finding

Elite performers deploy on demand (multiple times per day) AND have lower change failure rates than low performers. This refuted the conventional assumption that speed and stability trade off against each other. Fast and reliable are correlated, not opposed.

## The 24 Capabilities

Beyond the metrics, Accelerate identifies 24 capabilities that drive [[software-delivery-performance]], grouped into:

- Technical practices (continuous delivery, trunk-based development, test automation, deployment automation)
- Architecture (loosely coupled, independently deployable)
- Product and process (team experimentation, customer feedback, visual work)
- Lean management and monitoring
- Cultural capabilities (Westrum organizational culture, learning culture)

## Research Methodology

Forsgren led the statistical methodology. The book explains the use of structural equation modeling (SEM) to establish causal claims from survey data — an unusually rigorous approach for practitioner-facing business books. This distinguishes Accelerate from advocacy-based DevOps texts.

## Intellectual Position

Accelerate is the "Coding War Games" of the DevOps movement — the moment when practitioner intuition became empirical claim. Tom DeMarco and Timothy Lister's Coding War Games (1984) proved that developer performance varied by factors of 10 and that environment mattered; Accelerate proves that delivery practices vary by factors of hundreds and that specific practices are causally linked to performance.

## Relationship to Other Works

The book validates the prescriptions of [[the-devops-handbook]] and [[continuous-delivery-book]]. The [[state-of-devops-report-series]] is the annual source data. The DORA program was subsequently acquired by Google in 2018 ([[google-acquires-dora-2018]]).
