---
id: contributor-license-agreements
title: "Contributor License Agreements"
type: practice
tags:
- cla
- dco
- legal
- copyright
- governance
- licensing
metadata:
  practice_type: legal
  originated_in: "Apache Software Foundation"
  related_practices: &id001
  - code-review-in-foss
  - patch-based-development
  status: active
  research_status: draft
practice_type: legal
originated_in: "Apache Software Foundation"
related_practices: *id001
status: active
research_status: draft
---

A Contributor License Agreement (CLA) is a legal instrument that requires contributors to grant specific rights — either copyright assignment or a broad license — to a project or its governing entity before contributions are accepted. The CLA gives the receiving entity (typically a foundation or a company) clear legal standing to enforce the project's license, to relicense the software if strategic needs change, and to defend against intellectual property claims. The [[apache-software-foundation]] pioneered the modern CLA model for FOSS, requiring individual and corporate CLAs from all contributors to Apache projects. The Apache ICLA grants the ASF a perpetual, worldwide, non-exclusive license to use the contribution, while the contributor retains copyright.

The [[free-software-foundation]] takes a stronger approach: copyright assignment. Contributors to GNU projects assign their copyright to the FSF, which then holds unified copyright over the entire codebase. This gives the FSF maximum legal power to enforce the [[gpl-v2]] and [[gpl-v3]] — since it holds copyright on all contributions, it can pursue license violators without needing to coordinate with hundreds of individual copyright holders. [[richard-stallman]] argued that this concentration of copyright was necessary for effective copyleft enforcement. Critics counter that copyright assignment concentrates too much power in a single organization and creates a barrier for casual contributors who may be uncomfortable signing legal documents before submitting a bug fix.

The alternative to CLAs is the Developer Certificate of Origin (DCO), used by the Linux kernel since 2004. The DCO is a lightweight mechanism: contributors add a "Signed-off-by" line to their commit messages, certifying that they have the right to submit the code under the project's license. The DCO does not grant any additional rights beyond those already specified in the license — it simply establishes that the contributor is authorized to make the contribution. [[linus-torvalds]] adopted the DCO after the SCO litigation raised questions about the provenance of kernel code; the DCO provided a traceable chain of attestation without the bureaucratic overhead of a CLA. The DCO model has been adopted by many projects, particularly those under the [[linux-foundation]] umbrella.

The CLA controversy intensified during the [[mainstream-adoption-and-corporate-embrace-2005-2014]] era and into the [[modern-foss-and-sustainability-crisis-2015-present]] period as corporate-sponsored FOSS projects proliferated. When a company requires a CLA for an open source project it controls, the CLA can enable relicensing — the company can release future versions under a proprietary or more restrictive license because it holds broad rights over all contributions. This creates an asymmetry: community contributors grant rights to the company that the company does not reciprocate. Projects like MongoDB (before its shift to [[sspl-bsl]]) and Elasticsearch used CLAs that later facilitated license changes the community opposed. The result is a persistent tension in the FOSS ecosystem: CLAs provide genuine legal protection for projects, but they also enable the concentration of power that the movement's governance principles resist. The [[github-platform]]'s CLA bot integration made CLA enforcement easier, which simultaneously lowered friction for projects that use CLAs and increased the number of projects that require them.
