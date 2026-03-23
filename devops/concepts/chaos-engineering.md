---
id: chaos-engineering
title: "Chaos Engineering"
type: concept
importance: 6
tags:
- resilience
- netflix
- failure-injection
- testing
- production
concept_type: practice-category
first_appeared: "Netflix Chaos Monkey (2011); term formalized by Casey Rosenthal et al."
key_writings:
- site-reliability-engineering-book
related_concepts:
- site-reliability-engineering
- blameless-postmortems
- monitoring-and-observability
research_status: draft
---

Chaos engineering is the discipline of experimenting on a system in production to build confidence in its ability to withstand turbulent conditions. The defining characteristic is deliberate failure injection — not waiting for failures to occur randomly, but manufacturing them intentionally, in controlled ways, to understand system behavior and expose weaknesses before they matter.

## Netflix Origins

The origin is specific. In 2008, Netflix suffered a major database corruption that took the service down for three days. The event triggered a multi-year migration to AWS cloud infrastructure — a migration whose central operational challenge was: how do you maintain confidence in a system made of components that can fail at any time?

Netflix's response was Chaos Monkey, released internally in 2011 and open-sourced later. Chaos Monkey randomly terminated virtual machine instances in production during business hours. The logic: if instances will fail unexpectedly anyway, the engineers responsible for systems dependent on those instances should fix the failure modes now, under controlled conditions, rather than discover them during a 3 AM incident.

This inverted the traditional operations instinct — which is to prevent failures — in favor of expecting failures and engineering for resilience.

## From Chaos Monkey to the Simian Army

Netflix expanded the toolset into what they called the Simian Army: Chaos Monkey (instance termination), Chaos Gorilla (availability zone failures), Chaos Kong (region failures), Latency Monkey (network delay injection), Conformity Monkey (policy compliance checking). Each addressed a different failure category.

The evolution reflected increasing sophistication in failure taxonomy. Early chaos engineering focused on infrastructure failures (machines dying). Mature practice also addresses latency failures, dependency failures, data corruption, and human error scenarios.

Casey Rosenthal and Nora Jones formalized the discipline in "Chaos Engineering" (O'Reilly, 2020), establishing principles, methodologies, and the conceptual vocabulary. Rosenthal led Netflix's chaos engineering team and was positioned to describe the practice with both institutional authority and practitioner depth.

## Connection to the Second Way

In Kim's [[three-ways]] framework, chaos engineering is a Second Way mechanism. The Second Way is about feedback — creating fast, accurate signals about system health. [[monitoring-and-observability]] creates feedback from production behavior. Chaos engineering creates feedback from deliberate stress: it tells you how your system behaves under conditions you've engineered, before you experience those conditions accidentally.

This makes chaos engineering a form of hypothesis-driven experimentation: formulate a hypothesis about system behavior under a given failure condition, inject the failure, measure the outcome, update your understanding. The scientific method applied to production systems.

## The Philosophical Shift

The deeper significance is the philosophical reframing. Traditional operations assumes a steady state: systems should be up, failures are deviations to be prevented or repaired. Chaos engineering assumes turbulence is the normal state: failures will occur, the question is whether the system has been engineered to handle them gracefully.

This shift has precedents in resilience engineering (Erik Hollnagel, David Woods) and anticipatory failure determination. Resilience engineering asks not "why did this fail?" but "how does this system normally succeed despite complexity and variability?" Chaos engineering operationalizes that question as a practice.

## Game Days

Chaos engineering extends beyond automated failure injection into Game Days — planned exercises where teams deliberately simulate major failure scenarios (region outage, database unavailability, third-party dependency failure) in a controlled environment. Game Days involve people, process, and tooling simultaneously. They test incident response, communication protocols, and runbooks alongside technical resilience.

Game Days connect to the [[blameless-postmortems]] tradition: the failure is expected, the learning is the point, blame is inappropriate. Both practices share the same cultural prerequisite — an organization that treats failure as information rather than as evidence of negligence.

## Relationship to SRE

[[site-reliability-engineering]] practice includes chaos engineering as an advanced reliability discipline. The [[site-reliability-engineering-book]] references failure injection. The connection is direct: SLOs and error budgets define how much unreliability is acceptable; chaos engineering deliberately consumes some of that budget to produce knowledge about system behavior. Spending error budget on deliberate failures can prevent larger accidental failures later.
