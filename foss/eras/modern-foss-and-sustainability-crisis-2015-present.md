---
id: modern-foss-and-sustainability-crisis-2015-present
title: "Modern FOSS and the Sustainability Crisis (2015–Present)"
type: era
tags:
- sustainability
- maintainer-burnout
- sspl
- microsoft
- ai
- supply-chain
- open-weight-models
importance: 8
metadata:
  date_range: "2015-present"
  key_figures: &id001
  - nadia-eghbal
  - jim-zemlin
  - mitchell-baker
  key_writings: &id002
  - roads-and-bridges-2016
  - working-in-public-eghbal-2020
  key_concepts: &id003
  - maintainer-sustainability-crisis
  - open-core-business-model
  - software-freedom-vs-open-source
  - commons-based-peer-production
  - forking-as-governance
  key_events: &id004
  - microsoft-acquires-github-2018
  - xz-backdoor-2024
  research_status: draft
date_range: "2015-present"
key_figures: *id001
key_writings: *id002
key_concepts: *id003
key_events: *id004
research_status: draft
---

The period from approximately 2015 to the present has been characterized by the recognition that FOSS's infrastructural success created a sustainability problem the movement had not solved: the people who maintain critical software receive resources dramatically disproportionate to the value they produce. This era has also seen Microsoft's transformation from open source adversary to major participant, the rise of "source-available" licensing in response to cloud provider free-riding, and the emergence of AI/ML as the movement's next major contested frontier.

## The Sustainability Crisis Becomes Visible

The Heartbleed vulnerability (April 2014) was the alarm. OpenSSL — software securing a substantial fraction of internet traffic — was maintained by a small volunteer team with minimal funding. A serious memory safety bug had existed for over two years. After Heartbleed, the Core Infrastructure Initiative (later the Open Source Security Foundation, OpenSSF) was established to fund critical FOSS security work — the first major institutional response to the structural problem.

The left-pad incident (March 2016) exposed a different dimension: ecosystem fragility through dependency concentration. When developer Azer Koçulu unpublished 273 packages from npm (including the eleven-line `left-pad` module) in a dispute with Kik Interactive, thousands of JavaScript projects broke. An eleven-line utility that anyone could write in minutes had become a critical dependency for a large fraction of the Node.js ecosystem. The incident illustrated how the open source dependency model created systemic fragility alongside its benefits.

[[nadia-eghbal]]'s [[roads-and-bridges-2016]] (2016, funded by the Ford Foundation) provided the first comprehensive analysis of the sustainability crisis as a structural problem: FOSS was public infrastructure, but it was being maintained by volunteers without the funding mechanisms available to other public infrastructure. Her subsequent [[working-in-public-eghbal-2020]] (2020) analyzed the dynamics of open source maintenance — the asymmetry between maintainers and users, the attention costs of mass contribution — with the rigor the problem deserved.

## Microsoft's Transformation (2014–2018)

Under CEO Satya Nadella, Microsoft began a dramatic reversal of its historically adversarial posture toward open source. The company released .NET as open source (2014), created Visual Studio Code (an open source editor that became dominant), joined the Linux Foundation, and declared that "Microsoft loves Linux." The [[microsoft-acquires-github-2018]] — announced June 4, 2018 for $7.5 billion — was the most visible signal of this transformation.

The acquisition generated substantial community anxiety: GitHub was the critical infrastructure of FOSS collaboration, and it was now owned by a corporation with a history of hostility to open source. The anxiety proved partially well-founded and partially not: Microsoft has largely continued GitHub's operations and expanded its investment, but the dependency of the FOSS ecosystem on a single corporate-owned platform (one that is not itself open source) is a structural vulnerability that the acquisition made explicit. Some developers migrated to GitLab; Gitea and Forgejo represent community-owned alternatives that remain niche.

## Source-Available Licensing: The Cloud Provider Response

The SSPL and BSL (Business Source License) represented the attempt by commercial open source companies to close the cloud provider free-riding problem that the AGPL had not fully solved. MongoDB's relicensing under the SSPL in October 2018 was the most prominent instance. Redis, Elasticsearch, HashiCorp, and others followed with similar moves.

The OSI declined to certify the SSPL as an open source license — its provisions were considered incompatible with the [[open-source-definition]]. The licensing debate exposed a genuine tension: companies that had built on the FOSS model to attract developers and build communities felt that cloud providers (particularly AWS) were extracting value from their projects without contributing back or paying. The [[software-freedom-vs-open-source]] debate acquired a new dimension: some in the free software tradition argued that these companies were themselves trying to restrict user freedom, while the companies argued they were defending community sustainability.

## Supply Chain Security and the xz Backdoor (2024)

The [[xz-backdoor-2024]], discovered March 29, 2024, represented a qualitative escalation of supply chain security concerns. CVE-2024-3094 (CVSS 10.0) was a sophisticated, multi-year social engineering attack: a malicious actor using the identity "Jia Tan" had gradually built trust as a contributor to the xz Utils project, eventually becoming a de facto co-maintainer, and then inserted a backdoor targeting SSH authentication on systemd-based Linux systems. The attack was discovered by Andres Freund (Microsoft) who noticed anomalous SSH CPU usage and investigated.

The incident concentrated attention on several structural vulnerabilities: single-maintainer projects with no succession planning; the difficulty of evaluating the trustworthiness of contributors in anonymous, distributed communities; and the catastrophic potential of supply chain attacks against widely-deployed FOSS packages. It also illustrated the burnout dynamic: the xz maintainer had been under sustained pressure from fake users (apparently sock puppets operated by the attacker) complaining about the pace of development and demanding faster releases.

## AI/ML and the Open Source Frontier

The period from 2022 onward has seen AI/ML become a major contested domain for FOSS principles. "Open-weight" AI models (weights released for download and local use, but without training data or training code) have been described as "open source" by their developers and disputed as such by the FSF and others. Meta's LLaMA models, Mistral, and others occupy an ambiguous position: they enable substantial community use and modification but do not meet the [[four-freedoms]] criteria (particularly freedom 1: freedom to study how the program works, which requires training data and code as much as model weights).

The OSI published an "Open Source AI Definition" (v1.0, October 2024) that remains contested. The definitional battle over AI openness recapitulates the original free software vs. open source dispute with new stakes: if "open source AI" becomes standard terminology for models that do not meet free software criteria, it may further erode the meaning of both terms.

## What This Era Reveals

The modern era reveals that FOSS's success created a structural problem the movement had not designed for. The movement's institutions — the FSF, the OSI, the Apache Software Foundation — were built for a world where the challenge was adoption; they are not well-suited to the challenge of maintaining critical infrastructure under conditions of massive corporate appropriation and contributor burnout. The question that defines this era is whether the FOSS movement can develop the institutional and economic mechanisms to sustain the commons it created — or whether its most critical components will gradually be captured, abandoned, or weaponized.
