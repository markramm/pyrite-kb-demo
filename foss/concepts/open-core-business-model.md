---
id: open-core-business-model
title: "Open Core Business Model"
type: concept
importance: 6
concept_type: economic-model
first_appeared: "magic-cauldron-1999"
key_writings:
- magic-cauldron-1999
- roads-and-bridges-2016
- working-in-public-eghbal-2020
related_concepts:
- commons-based-peer-production
- maintainer-sustainability-crisis
- software-freedom-vs-open-source
tags:
- business-model
- commercialization
- sustainability
- cloud-providers
- licensing
research_status: draft
---

Open core is the dominant commercial model for FOSS companies from roughly 2008 onward: release a core product as open source to attract users, contributors, and ecosystem adoption, then sell proprietary extensions, enterprise features, hosted services, or support contracts to capture revenue. The model emerged from the failure of earlier FOSS business strategies — pure services (Red Hat), dual licensing (MySQL under GPL plus commercial license), and consulting — to scale reliably for most companies. [[magic-cauldron-1999]] surveyed the landscape of FOSS business models before open core became dominant, identifying the tension between value creation (which FOSS excels at) and value capture (which FOSS structurally resists).

The open core model requires a delicate calibration. The open source core must be valuable enough to attract a genuine user community and generate the network effects — documentation, integrations, bug reports, contributions — that make FOSS development powerful. But it cannot be so complete that no one needs the proprietary layer. MySQL (later Oracle), GitLab, Redis Labs, Elastic, and MongoDB all navigated versions of this balance. The proprietary additions typically include enterprise authentication, advanced monitoring, clustering, compliance features, or managed hosting — things that individual developers do not need but that enterprises require at scale. The result is a bifurcated product: a community edition that is genuinely open source under the [[mit-license]], [[apache-license-2]], or a copyleft license, and an enterprise edition that is proprietary software.

The model's central tension is philosophical as much as economic. From the [[software-freedom-vs-open-source]] perspective, open core is a pragmatic compromise: users get a useful open source tool, the company gets sustainable revenue, and the broader ecosystem benefits from the open core's existence. From the free software perspective, the proprietary layer is precisely the problem — it creates software that users cannot fully control, study, or modify, reintroducing the dependence that [[richard-stallman]] and the [[free-software-foundation]] defined the movement against. The [[open-source-initiative]] has generally accepted open core as compatible with the open source ecosystem, provided the core itself genuinely meets the [[open-source-definition]], but has drawn a firm line against labeling the proprietary extensions as "open source."

The open core model was disrupted starting around 2015-2018 by hyperscale cloud providers — primarily Amazon Web Services, but also Google Cloud and Microsoft Azure — who could take open-core products (Elasticsearch, Redis, MongoDB), offer them as managed services, and capture the hosting revenue without paying the vendor. The cloud providers argued they were exercising the rights granted by the open source license; the vendors argued this was free-riding that threatened their ability to fund development. This conflict drove MongoDB to adopt the [[sspl-bsl]] in October 2018, Elastic to adopt the Elastic License in 2021, and HashiCorp to adopt the Business Source License in 2023. Each of these moves was an implicit admission that the open core model had failed to protect the vendor's revenue stream against a sufficiently powerful competitor who could operate the software at greater scale than the original company.

The open core crisis connects directly to the [[maintainer-sustainability-crisis]]. When open core companies cannot sustain revenue, they face pressure to either restrict the open source core (eroding the community) or cut investment in maintenance (degrading the software). The FOSS ecosystem's dependence on venture-funded open core companies introduces a fragility: if the business model collapses, the open source project may be abandoned or relicensed, leaving users and contributors stranded. The OpenTofu fork (a [[linux-foundation]]-hosted fork of Terraform after HashiCorp's BSL relicensing in 2023) illustrates the community response: when a company retreats from open source, the right to fork — guaranteed by the original license — becomes the community's recourse. Whether forks can sustain themselves without the institutional backing of the original company remains an open question.
