---
id: three-ways
title: "The Three Ways"
type: concept
importance: 10
tags:
- foundational-framework
- lean-roots
- systems-thinking
- gene-kim
first_appeared: "Gene Kim's blog post (c. 2012) and The Phoenix Project (2013)"
key_writings:
- the-phoenix-project
- the-devops-handbook
- beyond-the-phoenix-project
related_concepts:
- continuous-delivery
- deployment-pipeline
- dora-four-key-metrics
- cams-framework
concept_type: framework
research_status: draft
---

The Three Ways is the organizing conceptual framework of the DevOps movement — the structure around which [[gene-kim]] built both [[the-phoenix-project]] and [[the-devops-handbook]], and the lens through which nearly every DevOps practice can be understood. Kim first articulated the framework in a 2012 blog post ([[the-goal-for-it]]) and then dramatized it through the character of Erik in The Phoenix Project. [[the-devops-handbook]] (2016) made it the explicit organizing principle for the entire handbook.

## The First Way: Flow

The First Way is about maximizing the rate of work flowing from Development through Operations to the customer — left to right through the value stream. It means:

- Making work visible (Kanban boards, deployment pipeline stages, queue lengths)
- Reducing batch sizes (small commits, feature flags, incremental delivery)
- Limiting work in progress
- Eliminating waste: handoffs, waiting, rework, unnecessary process
- Protecting the downstream workstation: never pass a known defect forward

The lean manufacturing root is direct: Taiichi Ohno's just-in-time production and value stream optimization. The First Way is lean flow applied to software delivery. [[continuous-delivery]] is the First Way's primary practical expression — the [[deployment-pipeline]] as the mechanism that makes flow visible and continuous.

## The Second Way: Feedback

The Second Way is about creating fast, amplified feedback loops flowing right to left — from production back through operations and into development. It means:

- Detecting problems as they occur (monitoring, alerting, telemetry)
- Stopping the production line when defects appear (andon cord analogy from Toyota)
- Building quality in at the source rather than inspecting it in at the end
- Pushing quality information upstream so developers can fix root causes

The Deming/TPS root: Deming's Plan-Do-Study-Act cycle, Toyota's jidoka (autonomation — machines that stop automatically when defects occur), and "stop the line" authority for any worker. Kim and [[john-willis]] both trace the Second Way explicitly to Deming's profound knowledge and W. Edwards Deming's observation that 94% of failures are system failures, not worker failures. [[blameless-postmortems]] are a Second Way practice: extract learning from failure rather than assign blame.

## The Third Way: Continual Learning and Experimentation

The Third Way is about building a culture of continual learning, experimentation, and improvement — converting individual learning into organizational learning, and making it safe to take calculated risks. It means:

- Allocating time for improvement work (not just feature delivery)
- Enabling experimentation even when it causes failure
- Creating institutional mechanisms to share what is learned (postmortems, internal wikis, communities of practice)
- Transforming local discoveries into global organizational improvements

The lean root is kaizen — continuous improvement as a never-ending practice, not a project. The Toyota kata: standardize, then improve the standard. [[chaos-engineering]] is a Third Way practice: deliberately introducing failure in controlled conditions to discover systemic weaknesses before they manifest as uncontrolled outages.

## Lean, Deming, and Goldratt Roots

The Three Ways distill three distinct intellectual traditions into a unified framework:

**First Way ← Lean flow**: Taiichi Ohno, the Toyota Production System, Womack and Jones's value stream mapping, Poppendieck lean software. [[gene-kim]] has explicitly mapped the First Way to muda (waste elimination) and mura (flow smoothing) from the three Ms of lean.

**Second Way ← Deming and TPS quality**: Deming's PDSA cycle, SPC (statistical process control), jidoka, andon cords. [[john-willis]]'s scholarly work on Deming's influence on DevOps traces this lineage in detail (see [[demings-journey-to-profound-knowledge]]).

**Third Way ← Kaizen and learning organization**: Deming's system of profound knowledge, Senge's learning organization, Toyota kata. The generative culture dimension draws on Ron Westrum's research on organizational culture in high-reliability organizations — which [[accelerate-book]] later validated empirically as a predictor of software delivery performance.

**Goldratt's TOC**: [[the-phoenix-project]] is structured as "The Goal for IT" — the same constraint-identification method, the same Socratic mentor structure. The Three Ways emerged from applying Goldratt's constraint-focused systems thinking to IT operations specifically.

## Organizing Role in DevOps

The Three Ways function as the conceptual scaffold for all of DevOps. Every DevOps practice can be mapped to one of the three:

- **First Way practices**: [[continuous-integration]], [[trunk-based-development]], [[deployment-pipeline]], [[deployment-automation]], [[version-control-everything]], [[feature-flags]], [[blue-green-deployments]], [[value-stream-mapping-for-it]]
- **Second Way practices**: [[monitoring-and-observability]], [[incident-management]], [[blameless-postmortems]], telemetry, on-call feedback loops
- **Third Way practices**: [[postmortem-practice]], [[chaos-engineering]], game days, improvement sprints, internal tech talks, open-source internal tooling

This mapping made the Three Ways a practical curriculum tool, not just a conceptual framework — it gave organizations a way to diagnose which dimension of DevOps they were weakest in.

## Relationship to CAMS and DORA

[[cams-framework]] (Culture, Automation, Measurement, Sharing) preceded the Three Ways and attempted a similar synthesis from a different angle. The two frameworks are complementary rather than competing: CAMS describes the categories of DevOps activity; the Three Ways describes the direction of flow and purpose of that activity.

[[dora-four-key-metrics]] provide the empirical measurement of whether the Three Ways are working: Deployment Frequency and Lead Time measure First Way outcomes; Change Failure Rate and MTTR measure Second Way effectiveness; improvement trends over time signal Third Way adoption.
