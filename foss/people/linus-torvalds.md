---
id: linus-torvalds
title: "Linus Torvalds"
type: person
tags:
- linux
- kernel
- git
- version-control
- bdfl
importance: 9
role: "Linux kernel creator, Git creator"
affiliations:
- linux-foundation
research_status: draft
---

Linus Torvalds (born 1969) created two pieces of software that became foundational infrastructure for the FOSS movement: the Linux kernel (1991) and the Git distributed version control system (2005).

The Linux kernel announcement in August 1991 — famously modest ("just a hobby, won't be big and professional") — initiated what became the largest collaborative software project in history. By the time Torvalds posted the announcement, Stallman's [[gnu-and-free-software-1983-1997]] project had produced most of the tools needed for a complete operating system; Linux supplied the missing kernel. Torvalds released Linux under the [[gpl-v2]], which he has consistently refused to upgrade to [[gpl-v3]], citing concerns about the anti-tivoization provisions and the involvement of patent clauses. "I'm an engineer, not a philosopher" is his characteristic stance on ideological questions.

Torvalds's governance model for the Linux kernel exemplifies [[bdfl-governance]]: he holds final commit authority and has maintained it for over three decades, even as thousands of contributors work through a lieutenant system of subsystem maintainers. His temperament — notoriously harsh in code review — became a flashpoint: in September 2018 he took a temporary leave to work on improving his behavior, and the kernel community adopted a formal Code of Conduct.

Git (2005) emerged from a practical crisis: the Linux kernel had been using the proprietary BitKeeper system, whose free license was revoked. Torvalds wrote Git in weeks as a replacement. Git's distributed model — every clone is a full repository — transformed how FOSS collaboration works, enabling [[github-platform]] and the pull-request workflow that now dominates the industry. The relationship between [[patch-based-development]] and Git-based development is one of the central transitions in modern FOSS practice.

Torvalds is employed by the [[linux-foundation]], which provides institutional support for his continued work on the kernel.

The [[bazaar-model]] described in [[cathedral-and-the-bazaar-1997]] was largely theorized from observing the Linux kernel development process, though Torvalds himself has rarely engaged with the theoretical literature about his project.
