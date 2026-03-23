---
id: feature-flags
title: "Feature Flags (Feature Toggles)"
type: practice
importance: 6
tags:
- delivery
- decoupling
- deployment-release-separation
- continuous-delivery
- dark-launch
practice_type: delivery
originated_in: "Flickr engineering practices (c. 2009); formalized in Continuous Delivery"
evidence_base: "DORA/Accelerate: enables trunk-based development and supports continuous delivery"
related_practices:
- trunk-based-development
- canary-releases
- deployment-automation
status: active
research_status: draft
---

Feature flags (also called feature toggles) are conditional switches in code that control whether a given feature is active at runtime, without requiring redeployment. A feature flag wraps new or incomplete functionality: the code is present in production, but the feature is invisible to users until the flag is switched on. Flags can be toggled per-environment, per-user cohort, per-percentage, or globally, depending on the flagging system.

## Origin: Flickr's Continuous Deployment

Feature flags are most directly associated with the deployment practices [[john-allspaw]] and [[paul-hammond]] described in their 2009 Velocity talk [[ten-deploys-per-day-talk]], which documented Flickr's practice of deploying to production ten or more times per day. Flickr maintained a feature flagging system that allowed them to deploy code continuously while controlling which users saw which features. This enabled dark launches, gradual rollouts, and instant kill switches without coordination delays.

[[continuous-delivery-book]] (Humble/Farley, 2010) formalized feature flags as a standard practice within the [[deployment-pipeline]], particularly as the mechanism that makes [[trunk-based-development]] safe: incomplete features in trunk are wrapped in flags and therefore harmless in production.

## Decoupling Deployment from Release

The central value of feature flags is the separation they create between two activities that, without flags, are necessarily coupled:

**Deployment**: the technical act of moving code from a version-controlled artifact into a running production system. With [[deployment-automation]], this becomes fast, low-risk, and frequent.

**Release**: the business act of making a feature available to users. This is a product decision, not a technical one: it depends on readiness, business timing, marketing coordination, and risk tolerance.

Without feature flags, every deployment is also a release. This conflation forces deployment frequency to match release frequency — which is typically low, because releases require coordination. Feature flags decouple the two, enabling [[continuous-integration]] and [[deployment-automation]] to operate at technical speed while releases happen at business speed.

## Use Cases

Feature flags serve multiple distinct purposes, which are sometimes conflated:

**Release flags**: hide incomplete features. The standard trunk-based development use case — the feature lives in production, switched off, until it is ready.

**Experiment flags** (A/B testing): different user cohorts see different versions of a feature. The flag controls assignment. Common in consumer products where data-driven product decisions require simultaneous deployment of multiple variants.

**Ops flags** (kill switches): flags that can disable a feature in production instantly if it causes problems. The kill switch is the inverse of a rollout — if a new feature degrades performance or produces errors, operations can disable it without a rollback deployment.

**Permission flags**: different users (beta users, internal users, paying tiers) see different features. More of a product configuration system than a deployment practice, but uses the same technical mechanism.

**Dark launches**: deploying a new code path and running it in production without surfacing results to users. Used to test performance and behavior under real load before any users are exposed.

## Connection to Trunk-Based Development

[[trunk-based-development]] depends on feature flags. Without flags, merging incomplete work to trunk risks exposing incomplete features to production users. Flags remove that risk: developers can commit partial implementations to trunk, where they are tested in the CI pipeline and eventually reach production, invisibly. This is the mechanism that makes continuous integration compatible with features that take longer than a day to build.

## Connection to Canary Releases

[[canary-releases]] use flag infrastructure to control rollout percentages. A canary is a feature flag set to a small percentage of traffic — say, 1% — with monitoring to detect problems before widening the rollout. Feature flag systems and canary release systems are sometimes distinct tools; in more sophisticated platforms (LaunchDarkly, Unleash, Flipt), they are unified.

## Operational Risks

Feature flags accumulate technical debt. Every flag is a branch in the codebase; many flags create an exponential space of possible code paths. Standard practice is to treat flags as temporary — set a cleanup date when creating a flag, and remove the flag and the conditional once the feature is fully rolled out and stable. Organizations that allow flag inventories to grow unmanaged often find themselves with hundreds of flags, some of which nobody understands or can safely remove. Martin Fowler's writing on feature toggles (2016) documented the taxonomy and cleanup discipline.

## Connection to First Way

[[three-ways]] First Way: feature flags enable continuous flow by removing the constraint that a feature must be complete before deployment. Work flows from development to production continuously; the feature flag mediates between the technical state (code in production) and the user-visible state (feature active). This is batch size reduction applied to the product dimension: instead of accumulating a large batch of features for a coordinated release, each feature flows continuously to production and is released when ready.
