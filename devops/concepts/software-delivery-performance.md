---
id: software-delivery-performance
title: "Software Delivery Performance"
type: concept
importance: 7
tags:
- dora
- empirical-research
- performance
- capabilities
- accelerate
concept_type: framework
first_appeared: "DORA research; codified in Accelerate (2018)"
key_writings:
- accelerate-book
- state-of-devops-report-series
related_concepts:
- dora-four-key-metrics
- three-ways
- continuous-delivery
research_status: draft
---

Software delivery performance is the measurable ability of an organization to deliver software quickly, reliably, and safely. The [[dora-research]] program and [[accelerate-book]] transformed it from a practitioner intuition into an evidence-based framework: specific capabilities drive software delivery performance, and software delivery performance predicts organizational performance.

## DORA's Central Contribution

Before [[accelerate-book]], DevOps advocacy rested on case studies and practitioner testimony: "we did this at Flickr/Netflix/Etsy and it worked." That evidence is meaningful but limited — it doesn't establish causality, it doesn't generalize statistically, and it's vulnerable to selection bias (maybe only exceptional organizations can do 10+ deploys per day).

[[nicole-forsgren]], [[jez-humble]], and [[gene-kim]] used four years of [[state-of-devops-report-series]] data — over 23,000 survey responses — and structural equation modeling to establish causal claims. The findings:

1. Software delivery performance is measurable via [[dora-four-key-metrics]] (Deployment Frequency, Lead Time for Changes, Change Failure Rate, Time to Restore Service)
2. Specific technical and organizational capabilities causally drive software delivery performance
3. Software delivery performance predicts organizational performance (profitability, market share, customer satisfaction, productivity)

Finding #3 is the strategic claim. DevOps is not just an operations efficiency play. Organizations that deliver software well outperform their industry peers on business metrics. This makes software delivery a strategic capability, not a technical implementation detail.

## The 24 Capabilities

Accelerate identified 24 capabilities that drive software delivery performance, grouped into five categories:

**Continuous Delivery**
- Use of version control for all production artifacts
- Deployment automation
- Continuous integration
- Trunk-based development
- Test automation
- Test data management
- Shift-left on security
- Loosely coupled architecture
- Empowered teams

**Architecture**
- Independently deployable, loosely coupled services

**Product and Process**
- Customer feedback loops
- Team experimentation
- Work visibility (value stream)
- Working in small batches

**Lean Management and Monitoring**
- Change approval process (lightweight)
- Monitoring [[monitoring-and-observability]]
- Proactive failure notification
- WIP limits
- Visualizing work

**Culture** (Westrum organizational culture)
- Supporting learning
- Climate for learning from failures
- Generative culture (high cooperation, risks shared, bridging encouraged)

## The Interconnection Finding

The most important implication of the 24 capabilities model: these capabilities are interconnected. You cannot cherry-pick one or two and expect the performance benefits. Trunk-based development requires continuous integration and test automation to be safe. Deployment automation requires loosely coupled architecture to work without coordination overhead. Blameless postmortems ([[blameless-postmortems]]) require a generative culture to be honest rather than performative.

The system must be approached as a system. This mirrors the [[three-ways]] framework — Flow, Feedback, and Learning reinforce each other; they are not independent levers. It also echoes Deming's point about driving fear out of organizations: if fear remains, quality data does not flow, and the measurement practices that are supposed to improve performance produce misleading numbers instead.

## Mapping to the Three Ways

The 24 capabilities cluster onto Kim's [[three-ways]] framework:

- **First Way (Flow)**: deployment automation, version control, CI, trunk-based development, small batches, loose coupling, deployment pipeline
- **Second Way (Feedback)**: monitoring and observability, continuous testing, customer feedback, proactive notification
- **Third Way (Learning)**: blameless postmortems, generative culture, learning climate, experimentation

Accelerate provides empirical weight behind the Three Ways: the capabilities that Kim prescribes are the same capabilities that DORA's research identifies as causally linked to performance. The two frameworks converge.

## Comparison to Coding War Games

Tom DeMarco and Timothy Lister's Coding War Games (documented in "Peopleware," 1987) proved that individual developer performance varied by a factor of 10:1 and that environmental factors — workspace quality, noise, interruption levels — were the primary predictors of performance. Individual talent was far less predictive than environment and practice.

Accelerate is the DevOps movement's Coding War Games. It proves that software delivery performance varies by orders of magnitude between high and low performers, and that specific organizational practices and capabilities — not individual talent or organizational luck — are the primary predictors. Both studies move the performance conversation from "hire better people" to "build better systems."
