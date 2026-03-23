---
id: monitoring-and-observability
title: "Monitoring and Observability"
type: practice
importance: 7
tags:
- monitoring
- observability
- feedback
- second-way
- dora-predictor
- telemetry
practice_type: monitoring
originated_in: "Systems administration tradition; formalized in DevOps through the Three Ways"
evidence_base: "DORA/Accelerate: monitoring and observability are strong predictors of software delivery performance"
related_practices:
- incident-management
- canary-releases
- deployment-automation
status: active
research_status: draft
---

Monitoring and observability are related but distinct disciplines for understanding the behavior of production systems. Monitoring collects predefined metrics and alerts when they cross thresholds — it tells you *when* something is wrong. Observability is the property of a system that makes it possible to understand its internal state from its external outputs — it is what allows you to answer *why* something is wrong, even for failure modes you did not anticipate. A system can be monitored without being observable; an observable system provides the foundation for effective monitoring.

## The Distinction That Matters

The monitoring-vs-observability distinction became a significant point of discussion in the DevOps and SRE communities during the 2010s, particularly as distributed systems became the norm.

Traditional monitoring assumes you know what to watch. You define: CPU should stay below 80%; error rate should stay below 0.1%; response time should be below 200ms. Alerts fire when thresholds are crossed. This works well for failures you have seen before and instrumented for. It fails for novel failure modes — which are, by definition, the ones that most need investigation in complex distributed systems.

Observability, as adapted into software engineering from control theory (the term originated in Rudolf Kálmán's 1960 work on linear systems), asks a different question: can you reconstruct the internal state of the system from its outputs, without modifying it? If you can, you can diagnose failures you have never seen before, because you have enough information to reason about what happened.

Charity Majors, Baron Schwartz, and Liz Fong-Jones (in their 2022 book *Observability Engineering*) formalized this distinction for software engineering practice and argued that traditional metrics-based monitoring is insufficient for modern distributed systems.

## The Three Pillars

The observability community converged on three signal types — often called the "three pillars":

**Logs**: structured records of discrete events — what happened, when, in what context. Logs are the oldest form of telemetry; the challenge is volume, indexing, and making them searchable and correlatable across distributed services.

**Metrics**: numerical measurements over time (counters, gauges, histograms). Metrics aggregate well and are efficient at scale; their limitation is that they discard the detail that would explain individual anomalies. Prometheus popularized a pull-based metrics model; Datadog, New Relic, and similar platforms provide hosted metric collection.

**Traces**: records of a single request's path through a distributed system — which services it touched, how long each took, where it failed. Tracing is the signal type most distinctive to distributed systems. Jaeger and Zipkin (2016) were early open-source distributed tracing systems; OpenTelemetry (2019) has emerged as the standard instrumentation framework.

The "three pillars" framing is critiqued as an oversimplification — Majors et al. argue that high-cardinality, structured events (from which logs, metrics, and traces can all be derived) are the more fundamental primitive — but the pillars remain a useful organizing framework.

## Tooling Evolution

Monitoring tooling has progressed through generations:

- **Nagios** (1999): the dominant open-source monitoring system for a decade. Checks defined as scripts; alerts via email. Effective for server-level health checks; not designed for distributed systems.
- **Graphite** (2006, Orbitz): time-series metric storage and graphing. The first widely-used tool for custom application metrics.
- **StatsD** (2011, Etsy): a simple UDP protocol for applications to emit metrics. Made it easy to instrument application code to send metrics without blocking on network calls.
- **Prometheus** (2012, SoundCloud): open-source monitoring with a pull-based collection model and a powerful query language (PromQL). Became the dominant open-source metrics system and the foundation of the CNCF monitoring ecosystem.
- **ELK Stack** (Elasticsearch + Logstash + Kibana): a popular log aggregation and search stack.
- **Distributed tracing**: Zipkin (2012, Twitter), Jaeger (2016, Uber), Honeycomb (2016) — focused on distributed traces rather than metrics.
- **OpenTelemetry** (2019): a merger of OpenTracing and OpenCensus, providing vendor-neutral instrumentation APIs for all three signal types.
- **Hosted platforms**: Datadog, New Relic, Dynatrace — commercial platforms that integrate monitoring, alerting, and observability into managed services.

## Connection to the Second Way

[[three-ways]] Second Way: monitoring and observability are the primary implementation of the Second Way in production. The Second Way demands fast, amplified feedback loops from production to development. Without telemetry, feedback from production is limited to user complaints and postmortem analysis. With comprehensive observability, feedback is continuous and quantitative: developers can see the effect of their changes in production within minutes of deployment.

This is the mechanism behind [[canary-releases]]: canary analysis requires metrics that distinguish the canary from the baseline. Without observability, canary analysis is blind. Similarly, [[incident-management]] requires observability to investigate incidents rather than merely detect them.

## DORA Evidence

[[accelerate-book]] identifies monitoring and observability as strong predictors of software delivery performance. High performers have proactive monitoring — they instrument their systems extensively and use telemetry to inform development decisions, not just to detect outages. The causal mechanism: observability reduces Mean Time to Restore (MTTR), one of the [[dora-four-key-metrics]]. When something fails, observable systems allow faster diagnosis and therefore faster recovery.

[[state-of-devops-report-series]] has consistently found that high performers are more likely to have monitoring and observability in place as a culture, not just a tool — engineers across development and operations share responsibility for instrumentation.

## SRE Connection

[[site-reliability-engineering]] at Google placed particular emphasis on monitoring design. The SRE Book's chapter on monitoring distributed systems introduced the concepts of **symptoms vs. causes** in alerting (alert on user-visible symptoms, not internal causes), **service level indicators** (SLIs), **service level objectives** (SLOs), and **error budgets** — a framework for making monitoring actionable in terms of user experience rather than infrastructure metrics. This SLO/SLI framework has become a widely adopted approach to making monitoring decisions that balance reliability and velocity.
