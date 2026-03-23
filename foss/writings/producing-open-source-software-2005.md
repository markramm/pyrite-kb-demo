---
id: producing-open-source-software-2005
title: "Producing Open Source Software"
type: writing
importance: 6
writing_type: book
date: 2005-10-14
author: karl-fogel
publisher: "O'Reilly Media"
key_concepts:
- bazaar-model
- bdfl-governance
- release-management
- code-review-in-foss
- contributor-license-agreements
- bug-triage-and-tracking
tags:
- fogel
- project-management
- governance
- community-building
- practical-guide
research_status: draft
---

The definitive practical guide to running a free and open source software project. [[karl-fogel]] wrote the first edition in 2005 (O'Reilly), drawing on his experience with the Subversion project. A second edition followed in 2017. The book is licensed under Creative Commons Attribution-ShareAlike, making it freely available online — a practice that embodies its subject matter.

## Content and Scope

The book covers the full lifecycle of an open source project: choosing a license, setting up infrastructure (version control, bug trackers, mailing lists), establishing governance, managing community norms, handling contributors, release management, and dealing with common failure modes (project abandonment, governance crises, hostile forks).

Where [[cathedral-and-the-bazaar-1997]] made the philosophical and methodological case for open development, "Producing Open Source Software" is the operator's manual. It treats governance and community management as engineering problems with known solutions — not because community dynamics are mechanical, but because experienced practitioners had accumulated hard-won knowledge that deserved systematic treatment.

Key themes include:
- How [[bdfl-governance]] works in practice and what its limits are
- [[contributor-license-agreements]] and [[code-review-in-foss]] as trust infrastructure
- [[bug-triage-and-tracking]] as community health signals
- The importance of communication norms and public decision-making for legitimacy
- [[release-management]] as a signal of project health

## Significance to the Movement

The book arrived at a moment — the [[mainstream-adoption-and-corporate-embrace-2005-2014]] era — when open source had won the argument but practitioners were discovering that winning the argument didn't mean knowing how to run large-scale collaborative projects. Git had just been released ([[git-release-2005]]); GitHub would follow in 2008 ([[github-launch-2008]]). The infrastructure for collaboration was proliferating faster than the knowledge of how to use it well.

Fogel's book became the standard reference for project founders and contributed to the normalization of open source governance practices across the industry. Its CC BY-SA license meant it could be freely shared, quoted, and built upon — and the 2017 second edition updated the content for a post-GitHub world where [[patch-based-development]] had largely given way to pull-request workflows.

The book's limitations are those of any practitioner guide: it describes successful patterns without always explaining why they work, and it is more useful for projects starting from scratch than for understanding why established projects encounter specific governance failures.
