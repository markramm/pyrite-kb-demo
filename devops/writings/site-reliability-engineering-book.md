---
id: site-reliability-engineering-book
title: "Site Reliability Engineering: How Google Runs Production Systems"
type: writing
importance: 8
tags:
- site-reliability-engineering
- google
- production-operations
writing_type: book
date: 2016-03-23
author: betsy-beyer
coauthors:
- Chris Jones
- Jennifer Petoff
- Niall Richard Murphy
publisher: "O'Reilly Media"
key_concepts:
- site-reliability-engineering
research_status: draft
---

The codification of Google's approach to running production systems at scale, edited by Betsy Beyer, Chris Jones, Jennifer Petoff, and Niall Richard Murphy, with chapters contributed by practitioners across Google's SRE organization.

[[site-reliability-engineering]] (SRE) as Google defines it: software engineering applied to operations problems. Google's answer to the dev-ops boundary problem was to hire software engineers to do operations work, with the explicit rule that no more than 50% of their time could be spent on operational toil.

## Core Concepts

**Error Budgets**: If a service has a 99.9% availability SLO (Service Level Objective), it has a 0.1% error budget — the amount of downtime acceptable per period. When the error budget is exhausted, new feature releases stop until reliability is restored. This makes reliability a shared concern between dev and ops rather than a source of conflict.

**Service Level Objectives (SLOs)**: Precise targets for service behavior (latency, availability, error rate). Distinct from SLAs (contractual commitments with customers). SLOs define the reliability target; error budgets define what's spent.

**Toil**: Operational work that is manual, repetitive, automatable, tactical, and does not provide enduring value. SRE practice requires reducing toil — if toil exceeds 50% of an SRE's time, the system is broken.

**Eliminating Toil through Automation**: The software-engineering approach to operations means writing code to eliminate manual work, not just doing the work faster.

## Relationship to DevOps

SRE is frequently described as "one implementation of DevOps principles" — it achieves the same goals (faster delivery, greater reliability, shared ownership) through a different organizational structure. DevOps tends toward merged teams and shared responsibilities; SRE tends toward specialized software engineers who own reliability with defined interfaces to product development teams.

The relationship is complementary rather than competitive. [[the-devops-handbook]] references SRE concepts; [[accelerate-book]]'s research covers both DevOps and SRE organizations. The monitoring, observability, and incident management practices that SRE systematized have been broadly adopted in DevOps contexts regardless of organizational structure.

## Companion Volumes

Google subsequently published "The Site Reliability Workbook" (2018) and "Building Secure and Reliable Systems" (2020), extending the SRE framework. All three are available free online at sre.google.
