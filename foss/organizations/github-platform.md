---
id: github-platform
title: "GitHub"
type: organization
tags:
- hosting
- git
- pull-requests
- microsoft
- collaboration
importance: 7
org_type: hosting-platform
founded: "2008"
research_status: draft
---

GitHub is the hosting platform that transformed how FOSS collaboration works — making contribution accessible through a web interface and pull-request workflow that superseded [[patch-based-development]] — and became central infrastructure for the global FOSS ecosystem before its acquisition by Microsoft.

GitHub launched in April 2008, founded by Tom Preston-Werner, Chris Wanstrath, PJ Hyett, and Scott Chacon. Built on top of [[linus-torvalds]]'s [[git-release-2005|Git]] version control system, GitHub added a web UI, social features (watching, forking, starring), and most importantly the pull request: a mechanism for proposing changes from a forked repository that enabled contribution without direct repository access. This dramatically lowered the barrier to contributing to FOSS projects and reshaped what contribution meant in practice.

The effects on FOSS culture were profound. [[patch-based-development]] — sending diff files by email for maintainer review — had been the dominant contribution model from the 1980s through the 2000s. GitHub's pull-request workflow enabled a different contributor profile: casual contributors who could submit a single change without subscribing to mailing lists, understanding email-based review customs, or managing complex toolchains. The tradeoff analyzed in [[working-in-public-eghbal-2020]] followed directly: more contributors, lower average contribution quality, and higher maintainer burden managing the inflow.

GitHub grew to host the majority of the world's open source projects, making it simultaneously the most important FOSS infrastructure and a single point of dependency for the ecosystem. This concentration raised questions [[nadia-eghbal]] analyzed in terms of [[maintainer-sustainability-crisis]]: the platform extracted enormous value from FOSS projects it hosted without compensating maintainers.

Microsoft acquired GitHub in June 2018 for $7.5 billion — the [[microsoft-acquires-github-2018]] event that generated intense debate within the FOSS community. Microsoft had been a consistent opponent of open source through the 2000s (Steve Ballmer's "Linux is a cancer" statement) but had shifted strategy dramatically under Satya Nadella. The acquisition was seen as either confirmation of FOSS's mainstreaming (Microsoft now depended on it) or as a capture of FOSS infrastructure by a historically hostile corporation. GitHub Copilot (2021), Microsoft's AI code completion tool trained on GitHub repositories, renewed the controversy — triggering the [[software-freedom-conservancy]]'s "Give Up GitHub" campaign.

The [[xz-backdoor-2024]] incident — a sophisticated supply chain attack targeting the XZ Utils compression library maintained through GitHub — illustrated how concentration of FOSS infrastructure on a single platform creates systemic vulnerability.
