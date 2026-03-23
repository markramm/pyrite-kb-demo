---
id: maintainer-sustainability-crisis
title: "Maintainer Sustainability Crisis"
type: concept
importance: 7
concept_type: critique
first_appeared: "roads-and-bridges-2016"
key_writings:
- roads-and-bridges-2016
- working-in-public-eghbal-2020
- magic-cauldron-1999
related_concepts:
- commons-based-peer-production
- open-core-business-model
- software-freedom-vs-open-source
- bdfl-governance
tags:
- sustainability
- maintainer-burnout
- security
- infrastructure
- public-goods
- funding
research_status: draft
---

The maintainer sustainability crisis is the structural problem at the heart of the modern FOSS ecosystem: critical digital infrastructure depends on projects maintained by volunteers or small teams with no funding, institutional support, or succession planning proportional to their importance. The crisis is not a bug in FOSS but a predictable consequence of its economic structure — [[commons-based-peer-production]] excels at creating public goods but provides no mechanism for maintaining them once they become infrastructure that millions depend on. The term crystallized in the [[modern-foss-and-sustainability-crisis-2015-present]] era, though the underlying dynamics were present from the beginning.

The canonical incidents trace a pattern. The Heartbleed vulnerability (April 2014) revealed that OpenSSL — the cryptographic library securing a substantial fraction of the internet's encrypted traffic — was maintained by two people, one of whom worked on it full-time with minimal funding. A critical buffer over-read bug had been present for two years in software that governments, banks, and technology companies relied on for security. The left-pad incident (March 2016) demonstrated a different fragility: a single developer, Azer Koculu, unpublished a trivial 11-line npm package in a dispute with the npm registry, breaking thousands of JavaScript builds including those of major companies. And the [[xz-backdoor-2024]] — the most consequential incident — showed that the crisis is not merely a sustainability problem but a security problem: a sophisticated attacker exploited a burned-out solo maintainer's need for help, spending two years building trust before inserting a backdoor into a compression utility present on virtually every Linux system. Each incident confirmed the same diagnosis: the FOSS commons is load-bearing infrastructure maintained under conditions that would be considered negligent in any other domain.

[[nadia-eghbal]]'s [[roads-and-bridges-2016]], commissioned by the Ford Foundation, gave the crisis its defining metaphor: open source software is digital infrastructure analogous to roads and bridges, critical and load-bearing but systematically underfunded because its public-good nature means the market undersupplies maintenance. The report shifted the conversation from individual project survival ("how does this project get funded?") to systemic infrastructure investment ("how does the commons as a whole get maintained?"). Eghbal's subsequent [[working-in-public-eghbal-2020]] deepened the analysis, arguing that the dynamics of the [[github-platform]] era had transformed most FOSS projects from community-produced commons into one-to-many media: a small core of maintainers producing for a vast audience of passive consumers whose "contributions" often increase the maintainer's burden rather than sharing it.

The crisis manifests in three interconnected forms. First, burnout: maintainers leave projects they created because the demands of issue triage, pull request review, dependency management, and user support overwhelm unpaid volunteer capacity. [[guido-van-rossum]]'s 2018 resignation as Python's BDFL — "I'm tired, and need a permanent vacation" — after a contentious PEP debate is a high-profile instance, but the pattern is pervasive in smaller projects. Second, security risk: unmaintained or under-maintained software accumulates vulnerabilities that no one reviews or patches, and the social trust model that makes FOSS contribution work provides attack surfaces for adversaries willing to invest time in building credibility, as the [[xz-backdoor-2024]] demonstrated. Third, inequality: corporations extract enormous value from FOSS — the entire cloud computing industry runs on Linux, Kubernetes, PostgreSQL, and thousands of smaller projects — while the maintainers of those projects work unpaid or underpaid, creating what Eghbal called a "free-rider problem at civilizational scale."

Institutional responses have diverged along the [[software-freedom-vs-open-source]] axis. The [[linux-foundation]]'s Open Source Security Foundation (OpenSSF, founded 2020) represents the corporate-pragmatist approach: companies that depend on FOSS infrastructure co-invest in security auditing, maintainer support, and supply chain tooling. The [[software-freedom-conservancy]] represents the freedom-centered approach: GPL enforcement, fiscal sponsorship for community-governed projects, and advocacy for maintainer rights. GitHub Sponsors, Open Collective, and Tidelift represent platform-mediated approaches that treat maintainers as creators deserving patronage. None of these has solved the structural problem. The crisis persists because the economic logic of [[commons-based-peer-production]] — low barriers to use, high barriers to funding — is inherent in the model, not a market failure that better institutions can straightforwardly correct.
