---
id: dora-four-key-metrics
title: "DORA Four Key Metrics"
type: concept
importance: 10
tags:
- empirical-research
- metrics
- software-delivery-performance
- accelerate
first_appeared: "State of DevOps Reports (2014-2018), codified in Accelerate (2018)"
key_writings:
- accelerate-book
- state-of-devops-report-series
related_concepts:
- software-delivery-performance
- three-ways
- continuous-delivery
concept_type: metric
research_status: draft
---

The DORA Four Key Metrics are the empirically derived measures of software delivery performance that emerged from the [[state-of-devops-report-series]] and were codified in [[accelerate-book]] (2018). They represent the field's most rigorous answer to the question: what should we measure to know whether our DevOps practices are working?

## The Four Metrics

**Deployment Frequency (DF)**: How often an organization deploys code to production. Elite performers deploy on-demand, multiple times per day. Low performers deploy monthly to every six months. DF is a proxy for batch size — high frequency means small batches, which means faster learning and lower risk per deployment.

**Lead Time for Changes (LT)**: The time from a code commit to that code running in production. Elite performers achieve lead times of less than one hour; low performers measure in months. Lead time captures the speed of the entire delivery system — testing, approval processes, deployment steps, environment constraints.

**Change Failure Rate (CFR)**: The percentage of changes to production that result in a degraded service requiring remediation (rollback, hotfix, patch). Elite performers maintain 0-15% CFR; low performers see 46-60% failure rates (approximate figures based on DORA cluster analysis; exact thresholds have shifted across report years).

**Mean Time to Restore (MTTR)**: The time to restore service when a production incident occurs. Elite performers restore in less than one hour; low performers take one to six months. MTTR measures the effectiveness of monitoring, incident response, and rollback capability.

## Why These Four

The selection of these four metrics is deliberate: they capture both throughput and stability dimensions of delivery performance, preventing local optimization on one dimension at the expense of the other.

- **Speed metrics**: DF and LT measure how fast value flows to users (First Way of [[three-ways]])
- **Stability metrics**: CFR and MTTR measure how well the system detects and recovers from failure (Second Way)

A team could theoretically score well on speed by deploying broken code frequently — CFR and MTTR expose this. A team could theoretically score well on stability by deploying rarely — DF and LT expose this. The four metrics together are harder to game than any single metric.

## The Central Finding: Speed and Stability Are Not Tradeoffs

The single most important finding from the DORA research is that high-performing organizations outperform low performers on ALL four metrics simultaneously. Elite performers deploy more frequently AND have lower change failure rates AND restore faster. This directly contradicts the intuitive assumption (and conventional IT management practice) that speed and stability trade off against each other.

This finding has the character of a paradigm shift: if the intuitive model were true, organizations managing the speed-stability tradeoff would be doing the right thing by going slowly. The DORA evidence shows the intuitive model is wrong — the practices that increase speed also increase stability, because they reduce batch sizes, increase feedback, and build quality in earlier.

## Evidence Base

The metrics emerged from four-plus years of the [[state-of-devops-report-series]], encompassing more than 23,000 survey responses from technology professionals worldwide. [[nicole-forsgren]] led the statistical methodology, using structural equation modeling (SEM) to establish causal relationships rather than mere correlation — an unusually rigorous approach for practitioner-facing research.

The [[dora-research]] program was acquired by Google in 2018 ([[google-acquires-dora-2018]]), continuing as an independent research program within Google Cloud.

## Cluster Analysis: Performance Tiers

The DORA research uses cluster analysis to identify distinct performance tiers:

- **Elite**: Deploy on-demand; lead time under one hour; CFR 0-15%; MTTR under one hour
- **High**: Deploy weekly to monthly; lead time one day to one week; CFR 16-30% (approximate)
- **Medium**: Varying performance on speed; higher CFR and MTTR
- **Low**: Monthly to semi-annual deployments; lead time one to six months; CFR up to 60%

The gap between elite and low performers is measured in orders of magnitude — 973x faster deployment frequency and 6,570x faster lead time were among figures reported in specific research iterations (approximate; figures vary by year).

## Relationship to the 24 Capabilities

[[accelerate-book]] identifies 24 technical, architectural, process, and cultural capabilities that drive the four key metrics. The capabilities most strongly predictive of high performance include:

- [[continuous-delivery]] practices (version control, trunk-based development, test automation, deployment automation)
- Loosely coupled, independently deployable architecture
- Westrum generative organizational culture
- Lean management practices
- [[monitoring-and-observability]]

This means the metrics are not merely measurement artifacts — they are outcome measures of a coherent set of causal practices.

## Comparison to Lean Metrics

The four metrics have direct lean manufacturing analogues:

- Deployment Frequency ↔ production rate / throughput
- Lead Time for Changes ↔ cycle time (time from order to delivery)
- Change Failure Rate ↔ defect rate / first-pass yield
- MTTR ↔ mean time to repair in manufacturing

The DORA metrics are, in this sense, the application of lean production measurement to software delivery. This connection is explicit in [[accelerate-book]]'s subtitle: "The Science of Lean Software and DevOps."

## Comparison to DeMarco and Lister

[[accelerate-book]] positions itself as the "Coding War Games" of the DevOps movement — a reference to Tom DeMarco and Timothy Lister's work in the 1980s that proved developer productivity varied by factors of 10 and that environment (not individual talent) was the primary driver. The DORA research does for delivery systems what Coding War Games did for individual developers: it proves that practices and organization matter, and that the variance between organizations is enormous and explainable.
