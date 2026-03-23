---
id: trunk-based-development
title: "Trunk-Based Development"
type: practice
importance: 7
tags:
- delivery
- branching
- small-batches
- dora-predictor
- xp-origins
practice_type: delivery
originated_in: "Extreme Programming practices; advocated in Continuous Delivery (2010)"
evidence_base: "DORA/Accelerate: trunk-based development (short-lived branches or no branches) is a predictor of software delivery performance"
related_practices:
- continuous-integration
- feature-flags
- deployment-automation
status: active
research_status: draft
---

Trunk-based development (TBD) is the practice of all developers committing to a single shared branch — "trunk" or "main" — either directly or through short-lived feature branches (typically less than one day old before merging). The trunk is always in a releasable state. Unfinished work is hidden behind [[feature-flags]] rather than isolated in long-lived branches.

## The Branching Problem TBD Solves

The dominant alternative to trunk-based development is feature branch development — keeping each feature in its own branch until it is complete, then merging. The Gitflow workflow (Driessen, 2010), which formalized the use of multiple long-lived branches (feature, develop, release, hotfix), became the dominant branching model for many teams during the 2010s.

The problem: long-lived branches defer integration. The longer a branch lives, the more the codebase diverges, the more painful the eventual merge, and the longer the feedback loop between writing code and discovering whether it integrates correctly. Integration risk accumulates silently in proportion to branch age.

TBD addresses this by making integration continuous rather than deferred.

## XP and Continuous Delivery Origins

The practice traces to [[continuous-integration]] as defined in XP: if developers commit frequently to a shared mainline, they are, by definition, not maintaining long-lived branches. [[jez-humble]] and [[david-farley]]'s [[continuous-delivery-book]] (2010) made the case explicitly: for a [[deployment-pipeline]] to work, the pipeline must have a single source of truth to build from. Multiple long-lived branches mean multiple pipeline runs in different states, which means you cannot know if your release candidate is what you think it is.

## Lean Connection: Small Batch Sizes

TBD is the software delivery instantiation of lean's small batch principle. Reinertsen's *Principles of Product Development Flow* (referenced across the DevOps canon) demonstrates mathematically that large batches increase variability, queue length, and total cycle time. A long-lived feature branch is a large batch: all the work accumulates and is delivered at once. Short-lived commits are small batches: continuous flow of small, validated increments.

[[three-ways]] First Way: TBD is how you eliminate the waste of deferred integration and achieve continuous flow in the development stage of the value stream.

## Feature Flags as the Enabling Technology

TBD requires the ability to deploy incomplete features safely. The solution is [[feature-flags]]: incomplete work ships to production but is switched off. This decouples deployment (technical act of moving code to production) from release (business act of making a feature available to users). Without feature flags, TBD forces either shipping incomplete features or deferring deployment — neither acceptable.

This means TBD and feature flags co-evolve as a system: you adopt one, you need the other.

## DORA Evidence

[[accelerate-book]] identifies trunk-based development as one of the technical practices that distinguish high performers from low performers. The finding: high performers either develop on trunk directly or use branches with lifetimes of less than one day. Low performers use long-lived branches (days to weeks). The correlation with [[dora-four-key-metrics]] is through Deployment Frequency and Lead Time — teams that integrate continuously can deploy more frequently with less lead time.

[[state-of-devops-report-series]] has tracked this finding across multiple years of survey data.

## Gitflow Critique

Gitflow created a branching model appropriate for versioned software with discrete releases (open-source libraries, packaged applications) and misapplied to web services and continuously deployed applications. For a service deployed to production multiple times per day, a release branch that lives for two weeks is organizational waste, not governance. The Gitflow model assumes releases are events; TBD assumes deployment is continuous.

The DevOps community's critique of Gitflow is not that branching is wrong, but that branching strategies designed for one deployment model are harmful when applied to another. The practice should match the delivery model.

## Organizational Preconditions

TBD is not always easy to adopt. Prerequisites:

- Fast [[continuous-integration]] builds (slow CI creates pressure to batch commits)
- Feature flag infrastructure ([[feature-flags]])
- A team culture that treats broken trunk as a stop-everything emergency
- Test coverage sufficient to give confidence that merging will not regress production

Organizations without these preconditions often adopt TBD and revert because they experience the pain of broken trunk without the infrastructure to make it safe.
