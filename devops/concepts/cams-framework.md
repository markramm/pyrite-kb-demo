---
id: cams-framework
title: "CAMS (Culture, Automation, Measurement, Sharing)"
type: concept
importance: 7
tags:
- devops-definition
- movement-history
- john-willis
- damon-edwards
first_appeared: "John Willis and Damon Edwards at first US DevOpsDays (Mountain View, 2010)"
key_writings:
- convergence-of-devops
related_concepts:
- three-ways
- dev-ops-cooperation
concept_type: framework
research_status: draft
---

CAMS is the first widely adopted framework for defining what DevOps means beyond tools and specific practices. It identifies four dimensions — Culture, Automation, Measurement, Sharing — that together characterize the DevOps approach. [[john-willis]] and [[damon-edwards]] introduced the acronym at the first US DevOpsDays in Mountain View in 2010 ([[first-us-devopsdays-2010]]), and it became the movement's first attempt at a definitional scaffold.

The CAMS framework is documented in [[convergence-of-devops]], Willis's 2012 historical essay on DevOps origins, which also traces the intellectual streams that converged to create the movement.

## The Four Pillars

**Culture**: DevOps begins with the elimination of the adversarial relationship between development and operations. The pre-DevOps organizational default was a wall: developers threw code over it, operations ran it, each group's incentives were misaligned with the other's. Culture as a CAMS pillar means shared responsibility for outcomes, blameless response to failure, psychological safety to surface problems, and organizational structures that reward cross-functional collaboration rather than silo optimization. This is the dimension that makes DevOps an organizational transformation rather than a tool adoption.

**Automation**: The entire delivery value stream — from code commit through test, build, and deployment — should be automated. Manual handoffs are waste: they are slow, error-prone, and opaque. Automation is the enabler of speed, reproducibility, and scale. The key automation practices: [[continuous-integration]], the [[deployment-pipeline]], [[deployment-automation]], and [[infrastructure-as-code]]. Automation is also what makes the other three pillars possible — without automated feedback (Measurement), human operators cannot act on information fast enough; without automated pipelines, Sharing knowledge about deployment becomes irrelevant.

**Measurement**: You cannot improve what you do not measure. The Measurement pillar means building comprehensive telemetry into systems, measuring the right things (outcomes, not just outputs), and using measurement to drive improvement rather than to assign blame. The [[dora-four-key-metrics]] represent the mature expression of this pillar: a small set of outcome metrics that capture delivery system performance and can be improved through specific practices. Without measurement, DevOps transformation is unmeasured sentiment; with measurement, it becomes a directed improvement program.

**Sharing**: Knowledge shared across teams and organizations creates a positive feedback loop. Sharing means: blameless postmortems shared openly within organizations; internal tech talks and documentation; open-source tooling; conference presentations (the [[devopsdays-conference]] and [[velocity-conference]] culture); blogs and public case studies. Sharing converts individual learning into community learning. It is the mechanism by which the DevOps movement grew — practitioners at Flickr, Etsy, Amazon, and Netflix shared what they learned, creating a cumulative knowledge base that others could build on.

## Origin and Context

The first US DevOpsDays was held in Mountain View, California in 2010, following the original [[first-devopsdays-ghent-2009]] organized by [[patrick-debois]] in 2009. Willis and Edwards were prominent in the DevOps Cafe podcast ([[devops-cafe-podcast]]) and early DevOpsDays organizing. The CAMS acronym emerged from their attempt to define DevOps in a way that was tool-agnostic and accessible to organizations asking "what is DevOps, actually?"

The timing matters: in 2010, "DevOps" was barely a year old as a term. There was no [[three-ways]], no [[dora-four-key-metrics]], no [[accelerate-book]]. CAMS was the first systematic attempt to answer the definitional question with something more than "Agile for operations" or "what Flickr does."

## CALMS: The Lean Extension

[[jez-humble]] later extended the acronym to CALMS by inserting **Lean** between Culture and Automation: Culture, Automation, Lean, Measurement, Sharing. The Lean pillar makes explicit what CAMS left implicit: the intellectual debt to lean manufacturing and the Toyota Production System. Lean practices — small batch sizes, value stream mapping, eliminating waste, limiting work in progress — are the operating principles that make Automation effective and give Measurement its context (measure against the lean baseline of waste and flow).

The CALMS version is more widely used in enterprise DevOps training and frameworks (it appears in the SAFe framework and various vendor documentation), though the Willis/Edwards CAMS formulation has historical priority.

## Relationship to the Three Ways

CAMS preceded [[three-ways]] (which appeared in Kim's 2012 blog post and [[the-phoenix-project]] in 2013) and attempted a similar synthetic function from a different angle:

- **CAMS** organizes DevOps by *type of activity* (cultural work, automation work, measurement work, knowledge sharing)
- **Three Ways** organizes DevOps by *direction and purpose of flow* (left-to-right flow, right-to-left feedback, continuous learning)

The two frameworks are complementary. CAMS is more useful for organizational assessment ("which of these four dimensions are we weakest in?"). The Three Ways is more useful for understanding why each practice exists ("which Way does this practice serve?").

Both frameworks reflect the same core insight: DevOps is not a tool category. It is a way of organizing work, feedback, and learning. CAMS established that insight in 2010, two years before the Three Ways gave it a systematic lean/Deming grounding.
