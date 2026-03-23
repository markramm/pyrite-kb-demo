---
id: github-launch-2008
title: "GitHub Launches (2008)"
type: event
tags:
- github
- git
- pull-request
- foss-infrastructure
- social-coding
- venture-capital
importance: 7
date: 2008-04-10
location: "San Francisco, California"
participants:
- github-platform
---

GitHub launched on April 10, 2008 (this date is approximate; April 2008 is well-established but the precise date varies across accounts). It was founded by Tom Preston-Werner, Chris Wanstrath, PJ Hyett, and Scott Chacon. The platform was initially bootstrapped without venture capital funding — Preston-Werner's revenue from Gravatar (a profile photo service he had sold) provided early capital — though GitHub later raised venture funding.

## The Pull Request Model

GitHub's central innovation for FOSS collaboration was the pull request: a structured workflow for proposing changes to a repository you do not own. The mechanics:

1. Fork a repository (create your own copy under your account)
2. Make changes in your fork
3. Open a pull request from your fork's branch to the upstream repository's branch
4. The upstream maintainer reviews, discusses, and merges or declines

This workflow existed in Git before GitHub — it was possible to do the same thing via email patches — but GitHub made it graphical, social, and accessible to people without command-line comfort. The pull request UI showed diffs, allowed line-by-line comments, tracked the discussion thread, and integrated with issue trackers.

The pull request workflow is now so standard that it shapes how developers think about collaboration even outside open source — the model has been adopted in internal enterprise development at most major technology companies.

## Social Coding and the Contribution Layer

GitHub added social features that made FOSS contribution legible in new ways: stars (bookmarking and popularity signals), watch/follow for activity feeds, contribution graphs (the "green squares" that visualize commit activity), and organizational pages. These features made a developer's open source activity visible as a professional portfolio, which changed the incentive structure for contribution.

The contribution graph, in particular, gamified open source activity in ways that had both positive (encouraging regular contribution) and negative (creating anxiety about "streaks," disadvantaging developers who contribute to private repos or whose work is not captured by GitHub metrics) effects.

## The Platform Concentration Problem

GitHub's success created a structural vulnerability for the FOSS ecosystem. By the mid-2010s, GitHub hosted the majority of significant open source projects. This concentration meant that:

- GitHub's terms of service decisions affect the entire FOSS ecosystem
- GitHub's reliability and uptime is a dependency for a large fraction of open source development
- GitHub's business decisions — including the [[microsoft-acquires-github-2018]] acquisition — have outsized consequences for the movement

The FOSS movement had built its collaboration infrastructure on a platform that was itself proprietary software, owned by a for-profit company, with no governance participation by the open source community. This was precisely the kind of institutional dependency that FOSS principles would suggest is problematic — but the network effects of GitHub made meaningful migration expensive.

## GitHub Copilot and Training Data Controversy

GitHub's release of Copilot (2021) — an AI code completion tool trained on GitHub-hosted code, including GPL-licensed repositories — generated significant controversy. Critics argued that training an AI on GPL code and using it to produce code without disclosure of the training data's origins violated the spirit (and potentially the letter) of copyleft licenses. The FSF commissioned a study; multiple lawsuits were filed. The Copilot controversy is part of the broader [[modern-foss-and-sustainability-crisis-2015-present]] era's AI/ML and open source tensions.

## Relationship to the FOSS Movement

GitHub's launch belongs to the [[mainstream-adoption-and-corporate-embrace-2005-2014]] era as a democratizing force that lowered contribution barriers and accelerated FOSS adoption. But its long-term consequence — concentration of FOSS infrastructure on a single proprietary platform, acquired by [[microsoft-acquires-github-2018]] — belongs equally to the [[modern-foss-and-sustainability-crisis-2015-present]] era as a case study in the risks of building a commons on proprietary infrastructure.

The tension between GitHub's genuine utility to the FOSS ecosystem and the structural problems it created has no clean resolution. The platform is indispensable and non-ideal simultaneously.
