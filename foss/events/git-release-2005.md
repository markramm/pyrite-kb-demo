---
id: git-release-2005
title: "Git Released by Linus Torvalds (2005)"
type: event
tags:
- git
- version-control
- linus-torvalds
- bitkeeper
- distributed-development
- github
importance: 8
date: 2005-04-07
location: "Helsinki, Finland"
participants:
- linus-torvalds
---

Git was first released by [[linus-torvalds]] in April 2005. The date given (2005-04-07) is approximate — the first public announcement and initial release occurred in early April 2005, with the first commit in the Git repository itself dated April 7, 2005. Git was developed in a remarkably short time: Torvalds wrote the initial version in approximately two weeks.

## Background: The BitKeeper Dispute

The Linux kernel had used BitKeeper, a proprietary distributed version control system, from 2002. BitKeeper's developer (Larry McVoy) provided free-of-charge licenses to Linux kernel developers, enabling the distributed development model the kernel needed. In April 2005, the free license was revoked after a dispute over Andrew Tridgell's reverse-engineering of the BitKeeper protocol (Tridgell was attempting to create a free alternative that could interoperate with BitKeeper repositories).

Torvalds faced an immediate problem: the kernel project needed version control, the existing free tools (CVS, Subversion) did not support the distributed model he required, and returning to BitKeeper was politically untenable. His solution was to write a new tool.

## Design Principles

Torvalds designed Git around several principles derived from his experience with BitKeeper and dissatisfaction with CVS:

- **Distributed**: Every clone is a full repository with complete history. There is no single authoritative server that must be available for developers to work.
- **Performance**: Git was designed from the start to handle the Linux kernel's scale — large history, many branches, frequent merges.
- **Data integrity**: Git uses SHA-1 (now SHA-256 in newer versions) content addressing, meaning every object in the repository is identified by a hash of its contents. This makes the history tamper-evident and enables reliable distributed synchronization.
- **Branching and merging**: Git treats branching and merging as first-class, low-cost operations — in contrast to systems like CVS where branches were expensive and merges were painful.

## Impact on FOSS Collaboration

Git's distributed model was directly enabling for the pull-request-based contribution workflow that [[github-launch-2008]] institutionalized. The key insight: if everyone has a full repository clone, anyone can make changes in their clone and propose them back to an upstream repository — without needing write access to the upstream. The patch-based workflow (email patches, apply with `git am`) predated GitHub, but GitHub's pull request interface made this workflow accessible to people who had never used a mailing list.

The transition from centralized version control (CVS, Subversion) to Git effectively changed who could contribute to open source projects. Contributing to a Subversion project required commit access from the project maintainers; contributing to a Git project required only the ability to clone the repository and propose changes via pull request or patch. This lowered barriers dramatically, though it also created the asymmetry between the large pool of contributors and the small pool of maintainers that [[nadia-eghbal]]'s [[working-in-public-eghbal-2020]] analyzed.

## Adoption Trajectory

Git adoption was rapid but not immediate. Through 2007-2008, Subversion remained dominant in many open source projects. [[github-launch-2008]] accelerated adoption by providing a compelling user interface and social layer on top of Git. By the mid-2010s, Git had become overwhelmingly dominant, displacing essentially all other version control systems in open source development and most of commercial development as well.

Git is licensed under [[gpl-v2]], consistent with the Linux kernel. This has occasionally created friction with projects that use permissive licenses and prefer their tooling to match.

## Relationship to the [[mainstream-adoption-and-corporate-embrace-2005-2014]] Era

Git's release is the opening event of the mainstream adoption era. The tool that enabled GitHub, which enabled the democratization of contribution, which enabled the corporate embrace of open source development — it traces back to a licensing dispute over a proprietary tool used by the Linux kernel project. The irony is characteristic of FOSS history: the movement's most transformative collaboration tool was created in response to a reminder that proprietary tools remain proprietary.
