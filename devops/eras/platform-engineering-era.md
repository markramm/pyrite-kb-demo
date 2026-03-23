---
id: platform-engineering-era
title: "Platform Engineering and Maturity (2018-present)"
type: era
importance: 6
tags:
- platform-engineering
- gitops
- cloud-native
- team-topologies
- internal-developer-platform
date_range: "2018-present"
key_figures:
- gene-kim
- nicole-forsgren
- steven-spear
key_writings:
- the-unicorn-project
- wiring-the-winning-organization
- investments-unlimited
key_concepts:
- five-ideals
- software-delivery-performance
---

The era in which DevOps became the default rather than the aspiration, raising new questions about what comes next, how to optimize at scale, and how to govern what the movement had built.

**DevOps as baseline.** By 2018, "should we do DevOps?" was no longer the question in most engineering organizations. CI/CD pipelines, cloud infrastructure, containerization, and some form of dev-ops integration had become standard. The discourse shifted: "DevOps is dead" commentary reflected not failure but maturation — the term was becoming too broad to be useful. This is how successful movements end up dissolving into the background of normal practice.

**Platform engineering.** The next evolution emerged in response to a problem created by DevOps success: if every team must build and maintain its own toolchain, the cognitive load becomes unsustainable. Platform engineering — building internal developer platforms (IDPs) that make DevOps capabilities self-service — addressed this. Rather than requiring every team to assemble and operate CI/CD, monitoring, and deployment infrastructure, platform teams provide it as a product. Team Topologies (2019, Matthew Skelton and Manuel Pais) provided the organizational framework, introducing platform teams as one of four fundamental team topologies.

**GitOps.** Weaveworks introduced the GitOps term (approximately 2017-2018) to describe using Git as the single source of truth for declarative infrastructure and application state. With Kubernetes as the execution layer, GitOps patterns became mainstream — pull-based deployment, drift detection, and reconciliation as the operational model.

**Organizational theory deepening.** [[gene-kim]]'s [[the-unicorn-project]] (2019) returned to narrative form but focused on developer experience and the [[five-ideals]]: locality and simplicity, focus, flow, and joy, improvement of daily work, psychological safety, customer focus, and flow. [[wiring-the-winning-organization]] (Kim and [[steven-spear]], 2023) engaged more directly with organizational systems theory. [[investments-unlimited]] (2023) addressed governance, audit, and compliance within DevOps — the compliance and risk functions that had been largely unaddressed in the movement's earlier phases.

**DORA at Google.** The [[google-acquires-dora-2018]] acquisition institutionalized the State of DevOps research program at Google Cloud (dora.dev). DORA's four key metrics evolved into DORA metrics as an industry standard, widely implemented in tooling. [[nicole-forsgren]] later moved to GitHub as VP of Research and Strategy — the empirical tradition she built continued across institutional contexts.

**Open questions.** The era surfaced tensions the founding community had not resolved: how to do DevOps in regulated industries, how to handle the compliance burden, whether the "you build it, you run it" model scales to very large organizations, and how platform abstraction changes the developer experience in ways that may recreate some of the original dev-ops separation problems.
