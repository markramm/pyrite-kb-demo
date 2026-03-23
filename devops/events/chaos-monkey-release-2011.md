---
id: chaos-monkey-release-2011
title: "Netflix Releases Chaos Monkey (2011)"
type: event
importance: 6
tags:
- chaos-engineering
- netflix
- resilience
- aws
- fault-injection
date: 2011-07-19
location: "Netflix, Los Gatos, California"
participants: []
significance: "Pioneered chaos engineering — deliberately injecting failure to build resilience"
research_status: draft
---

July 2011. Netflix announced Chaos Monkey in a blog post by Yury Izrailevsky and Ariel Tseitlin. The tool randomly terminated production instances on AWS to test whether Netflix's systems could survive — and recover from — unexpected failures. It became the founding artifact of [[chaos-engineering]] as a discipline.

**The backstory.** Netflix had migrated from its own data centers to AWS beginning around 2008-2009, following a database corruption event in 2008 that caused a three-day outage affecting DVD shipments. The migration to cloud was also a forced reckoning with distributed systems failure modes — on AWS, individual instances would fail, regions would have issues, dependencies would become unavailable. The question was whether Netflix's architecture was actually as resilient as they believed, or whether resilience was assumed rather than tested.

Chaos Monkey operationalized a simple answer: if you want to know if your system handles random instance failures, introduce random instance failures deliberately — in production, during business hours, when engineers are present to respond. The alternative (waiting for failures to happen on their own) left the system untested under real conditions.

**The Simian Army.** Chaos Monkey was open-sourced in 2012 under the Apache 2.0 license and became the seed of the "Simian Army" — a collection of tools for testing different failure modes: Chaos Gorilla (availability zone failure), Latency Monkey (network latency injection), Conformity Monkey (checking configuration compliance), Janitor Monkey (resource cleanup). Each addressed a different class of production risk.

**Formalization of the discipline.** Chaos engineering as a named discipline was formalized later by Netflix engineers, culminating in the "Principles of Chaos Engineering" (principlesofchaos.org, approximately 2014-2016) and Casey Rosenthal et al.'s "Chaos Engineering" (O'Reilly, 2020). The discipline spread beyond Netflix — GameDay practices, chaos platforms (Gremlin, Chaos Toolkit), and integration into SRE practice at major organizations.

**Relationship to DevOps.** Chaos engineering sits at the intersection of [[site-reliability-engineering]] and DevOps. The underlying premise — that systems should be validated under adversarial conditions, that production is the only ground truth — is consistent with the DevOps emphasis on feedback loops and [[monitoring-and-observability]]. The [[blameless-postmortems]] culture that DevOps advocates for is a prerequisite for chaos engineering: teams must be able to intentionally cause failures without fear of blame.
