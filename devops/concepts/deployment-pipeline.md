---
id: deployment-pipeline
title: "The Deployment Pipeline"
type: concept
importance: 8
tags:
- automation
- continuous-delivery
- value-stream
- foundational-pattern
first_appeared: "Continuous Delivery (Humble/Farley, 2010)"
key_writings:
- continuous-delivery-book
- the-devops-handbook
related_concepts:
- continuous-delivery
- continuous-integration
- infrastructure-as-code
concept_type: pattern
research_status: draft
---

The deployment pipeline is an automated manifestation of the process for getting software from version control into the hands of users. It is the central mechanism of [[continuous-delivery]] — the concrete engineering artifact that makes the First Way ([[three-ways]]) operational. Every code change flows through a defined sequence of automated stages; the pipeline's job is to ensure that only changes meeting quality standards can reach production, and to do so as fast as possible.

[[jez-humble]] and [[david-farley]] codified the concept in [[continuous-delivery-book]] (2010). The concept had existed in nascent form in high-performing organizations (Flickr's deployment process is documented in [[ten-deploys-per-day-talk]]), but Humble and Farley gave it a systematic architecture applicable from first principles.

## Pipeline Stages

A canonical deployment pipeline passes every code change through progressively slower, higher-fidelity stages:

**Commit Stage**: Triggered on every commit to the main branch. Compiles code, runs unit tests, runs static analysis, produces deployable artifacts. Must be fast — under 10 minutes is a common target — so feedback reaches developers while context is still fresh. A failed commit stage stops the pipeline; nothing proceeds to downstream stages.

**Acceptance Test Stage**: Runs automated acceptance tests (functional, behavioral) against the artifact produced by the commit stage. Slower than unit tests; may take tens of minutes. Tests the system from the outside, validating that it meets business requirements.

**Performance/Capacity Testing Stage**: Validates that the system meets non-functional requirements under load. Often run less frequently than acceptance tests due to cost and time.

**Manual Exploration/UAT Stage**: Optional stage where humans test the system before production release — exploratory testing, UX review, stakeholder sign-off. At high CD maturity, this stage shrinks or disappears as automated coverage increases.

**Production Deployment**: The push of a button — or, in Continuous Deployment, an automatic trigger — that releases the artifact to production.

The key property: every stage must pass before the next stage runs. A defect caught in the commit stage never reaches acceptance testing. A defect caught in acceptance testing never reaches production. The pipeline embodies the First Way injunction never to pass a known defect downstream.

## Pipeline as Value Stream

The pipeline is the value stream for software delivery. This mapping is explicit in lean terms:

- **Inventory**: code committed but not yet deployed is work-in-progress inventory
- **Cycle time**: the end-to-end time from commit to production is the delivery cycle time
- **Throughput**: deployment frequency is the throughput of the delivery value stream
- **Defects**: change failure rate is the quality yield of the pipeline

[[value-stream-mapping-for-it]] applied to software delivery reveals the pipeline's structure and, more importantly, reveals where work queues up and waits — the constraints in Goldratt's Theory of Constraints sense. [[the-devops-handbook]] uses value stream mapping to diagnose pipeline bottlenecks: environments that take hours to provision, test suites that take days to run, approval processes requiring multiple sign-offs.

## Pipeline as Constraint Revealer

The pipeline makes constraints visible in a way that pre-pipeline operations did not. If work queues at the acceptance test stage — if a hundred builds are waiting to run acceptance tests — the pipeline has identified the system constraint. Goldratt's TOC (see [[the-goal-for-it]]) prescribes: identify the constraint, exploit it, subordinate everything else to it, elevate it. For a pipeline constraint, this means: make the slow test stage faster (parallelize, trim test count), ensure the constraint stage never sits idle (prioritize it over other work), and do nothing that creates more work for it to process.

This constraint-making-visible function is part of why the pipeline is a management tool, not just a technical tool. [[the-phoenix-project]]'s character Brent — the indispensable engineer who is the constraint in every work stream — is the human equivalent of a pipeline bottleneck.

## Pipeline as the Mechanism Enabling CD

Without the pipeline, [[continuous-delivery]] is a statement of intent with no implementation. The pipeline is what makes the definition of CD ("every change that passes can be released at any time") operationally real:

- Every change is tested automatically — there is no manual quality gate that creates a batch
- The artifact produced by the pipeline is known-good — it passed all gates
- Deployment is a push-button operation on a pre-validated artifact — not a high-risk manual process
- The pipeline provides the [[dora-four-key-metrics]] in natural form: DF is the number of pipeline completions, LT is the pipeline duration, CFR is the proportion of deployments that cause incidents, MTTR is measured from incident to recovery

## Extension to Infrastructure

[[the-devops-handbook]] extends the pipeline concept beyond application code to encompass [[infrastructure-as-code]]: the same pipeline that builds and tests application code also provisions, configures, and tests the infrastructure that runs it. This means:

- Infrastructure changes flow through the same quality gates as application changes
- Infrastructure code is version-controlled, tested, and deployed with the same discipline
- The pipeline tests the integrated system — application and infrastructure together — before production

This extension is the technical foundation for DevOps as a practice of shared responsibility rather than organizational role separation. If development and operations teams both commit to the same pipeline, both are accountable for the same quality gates.

## Humble and Farley's Codification

Before [[continuous-delivery-book]], the pipeline concept existed in practice at advanced organizations but without a name, systematic architecture, or guidance for implementation from scratch. Humble and Farley's contribution was:

1. Naming the concept and making it a first-class design artifact
2. Defining the stage structure and the principles governing each stage
3. Showing how to build it incrementally — starting with a minimal commit stage, then extending
4. Establishing the connection to lean concepts (small batches, single-piece flow, stop-the-line quality control)

The pipeline concept has proven durable: tools change (Jenkins → GitHub Actions → Tekton → cloud-native build systems), but the pipeline architecture Humble and Farley described remains the organizing pattern.
