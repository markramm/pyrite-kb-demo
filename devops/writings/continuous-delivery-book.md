---
id: continuous-delivery-book
title: "Continuous Delivery: Reliable Software Releases through Build, Test, and Deploy Automation"
type: writing
importance: 10
tags:
- foundational-text
- deployment-pipeline
- continuous-delivery
- infrastructure-as-code
writing_type: book
date: 2010-07-27
author: jez-humble
coauthors:
- David Farley
publisher: "Addison-Wesley"
key_concepts:
- deployment-pipeline
- continuous-delivery
- infrastructure-as-code
research_status: draft
---

The foundational technical text of the DevOps movement — written before the word "DevOps" had achieved widespread usage, but retrospectively recognized as the movement's most technically rigorous statement. Won the Jolt Award for best technical book.

[[jez-humble]] and [[david-farley]] codified a set of practices that had been emerging from the Agile and XP communities, giving them a unified framework: the [[deployment-pipeline]].

## The Deployment Pipeline

The central contribution: the deployment pipeline is a sequence of automated stages through which every code change passes — build, unit test, acceptance test, performance test, production deployment. The pipeline makes the state of every change visible, catches defects early, and ensures that software is always in a releasable state.

This concept had existed in practice at places like Flickr (see [[ten-deploys-per-day-talk]]), but Humble and Farley gave it a systematic architecture and showed how to build it from first principles.

## Continuous Delivery vs. Continuous Deployment

The book draws a distinction that became important in the field:

- **Continuous Delivery**: every change that passes the pipeline can be released to production at any time (human decision required)
- **Continuous Deployment**: every change that passes the pipeline is automatically deployed to production

This distinction gave organizations a target that was achievable without requiring full automation of the release decision.

## Infrastructure as Code

The book also codified [[infrastructure-as-code]] as a core practice — the idea that infrastructure should be managed through version-controlled scripts and configurations rather than manual operations. This was the operational complement to the development-side practices from XP and Agile.

## Intellectual Lineage

The book draws heavily from XP (especially continuous integration, test-driven development) and extends it through the deployment boundary into operations. It synthesizes:

- Kent Beck's continuous integration
- Mary and Tom Poppendieck's lean software concepts (see Poppendiecks KB)
- Agile testing practices
- Unix/sysadmin automation traditions

## Relationship to DevOps

The book predates the "DevOps" label (coined at [[first-devopsdays-ghent-2009]]) but is recognized as the movement's technical bible. [[the-devops-handbook]] explicitly draws on it, and [[accelerate-book]] validates many of its core prescriptions empirically through the DORA research.

[[gene-kim]] has consistently described Continuous Delivery as the most important technical book of the DevOps movement.
