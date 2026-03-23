---
id: continuous-delivery
title: "Continuous Delivery"
type: concept
importance: 9
tags:
- deployment
- automation
- flow
- foundational-practice
first_appeared: "Continuous Delivery (Humble/Farley, 2010)"
key_writings:
- continuous-delivery-book
- the-devops-handbook
- accelerate-book
related_concepts:
- deployment-pipeline
- continuous-integration
- three-ways
concept_type: practice-category
research_status: draft
---

Continuous Delivery (CD) is the practice of keeping software in a perpetually releasable state — every change that passes the automated [[deployment-pipeline]] can be deployed to production at any time, by any authorized person, at the push of a button. It is the primary technical expression of the First Way ([[three-ways]]): flow from development to operations to the customer.

[[jez-humble]] and [[david-farley]] codified the concept in [[continuous-delivery-book]] (2010), synthesizing a set of practices that had been emerging in the XP and Agile communities but lacked unified treatment. The book predates widespread use of the term "DevOps" (which emerged from [[first-devopsdays-ghent-2009]]) but is retrospectively recognized as the movement's foundational technical text.

## Definition and Scope

Continuous Delivery means the software delivery system is in a state where:

1. Any change that passes the pipeline is deployable to production
2. Deployment is a low-risk, routine activity (not an event)
3. The release decision is a business decision, not a technical one
4. The pipeline provides fast, accurate feedback about the quality of every change

This is distinct from Continuous Integration (CI), which is a prerequisite: CI means all developers integrate their work to a shared mainline frequently (at least daily). CD extends CI through the delivery boundary into production.

## The CD/Continuous Deployment Distinction

[[continuous-delivery-book]] draws a distinction that became important in practice:

- **Continuous Delivery**: every change that passes the pipeline can be released to production at any time (a human decides when to release)
- **Continuous Deployment**: every change that passes the pipeline is automatically deployed to production without human intervention

Most organizations practice Continuous Delivery rather than Continuous Deployment. The distinction gave organizations an achievable goal: the technical challenge is building the capability, not automating the release decision. Some organizations (like Etsy and Amazon at high maturity) move toward Continuous Deployment over time.

## The Deployment Pipeline as Mechanism

The [[deployment-pipeline]] is the mechanism that implements Continuous Delivery. Without an automated, fast pipeline, CD is impossible — every change must flow through a repeatable, automated sequence of build, test, and deployment stages before it can reach production.

Prerequisites for CD are also prerequisites for a functional pipeline:

- **Version control everything**: application code, test code, infrastructure configuration, database schema migrations, documentation
- **Automated testing**: unit tests, integration tests, acceptance tests, smoke tests in production
- **Trunk-based development**: all developers commit to the main branch frequently (not long-lived feature branches that create integration problems)
- **Fast build and test cycles**: if the pipeline takes hours, developers stop committing frequently; if it takes minutes, they commit multiple times per day

## Lean and First Way Roots

Continuous Delivery is the First Way ([[three-ways]]) made operational. The lean manufacturing concepts that underpin the First Way map directly:

- **Small batch sizes**: frequent, small commits reduce risk per change and accelerate feedback
- **Single-piece flow**: each commit moves through the pipeline as a unit, not accumulated in releases
- **Eliminating inventory**: unreleased code is inventory — features built but not delivered to users
- **Just-in-time delivery**: software delivered close to when it is needed, not accumulated in quarterly releases

[[the-devops-handbook]] uses the concept of "deployable artifacts" moving through the pipeline in the same way lean manufacturing uses "work in process" — the pipeline makes inventory visible and creates pressure to reduce it.

## Humble and Farley's Contribution

Before [[continuous-delivery-book]], the practices that constitute CD existed in scattered form across the XP community (Kent Beck's continuous integration), the Agile testing community, and in the operational practice of advanced organizations like Flickr (see [[ten-deploys-per-day-talk]]). Humble and Farley did three things:

1. Named the capability as a coherent practice category
2. Provided the deployment pipeline as a unifying architectural concept
3. Showed how to build it from first principles, including the infrastructure-as-code dimension

[[gene-kim]] has described [[continuous-delivery-book]] as the most important technical book of the DevOps movement. It remains the primary reference for practitioners implementing CD.

## DORA Evidence

The [[state-of-devops-report-series]] and [[accelerate-book]] identify continuous delivery practices as among the strongest predictors of [[software-delivery-performance]]. The 24 capabilities in [[accelerate-book]] include multiple CD-specific capabilities:

- Use of version control for all production artifacts
- Deployment automation
- Continuous integration
- Trunk-based development
- Test data management
- Shift-left on security

Organizations that score high on these capabilities score high on [[dora-four-key-metrics]] — the empirical validation that CD's prescriptions are causally linked to performance, not merely associated with it.

## Relationship to Site Reliability Engineering

Google's [[site-reliability-engineering]] practice, developed in parallel with the DevOps movement, shares CD's emphasis on automation, pipeline-based deployment, and eliminating toil from operations. The SRE approach treats operations as a software engineering problem rather than a manual process — a parallel formulation of the same First Way logic from an operations-centric perspective.
