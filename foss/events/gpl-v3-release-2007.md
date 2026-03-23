---
id: gpl-v3-release-2007
title: "GPL Version 3 Released (2007)"
type: event
tags:
- gpl-v3
- copyleft
- tivoization
- software-patents
- richard-stallman
- fsf
- linux-kernel
importance: 7
date: 2007-06-29
location: "Boston, Massachusetts (FSF headquarters)"
participants:
- richard-stallman
- free-software-foundation
---

The GNU General Public License version 3 was released on June 29, 2007, by the [[free-software-foundation]] after an unprecedented three-year public drafting process. [[richard-stallman]] led the drafting, with legal counsel from Eben Moglen and the Software Freedom Law Center. The release marked the FSF's most significant legal innovation since the original GPL, but also highlighted the growing divergence between the FSF's ethical free software vision and the direction of the broader open source ecosystem.

## Background: Problems GPL v2 Had Not Anticipated

[[gpl-v2]] was written in 1991, before two developments that [[richard-stallman]] and the FSF considered serious threats to software freedom:

**Tivoization**: TiVo's digital video recorders ran a Linux-based system (and thus GPL v2 code) but used cryptographic verification to prevent users from running modified versions of the software on the device. The device would verify the software's signature at boot; unsigned (modified) software would be rejected. TiVo was technically compliant with GPL v2 — it provided source code — but users could not exercise the freedom GPL v2 was meant to protect: the freedom to run modified versions of the software on their own hardware. Stallman coined the term "tivoization" for this practice.

**Software patents**: GPL v2's interaction with software patent licenses was unclear. A company could distribute GPL v2 software under a patent license that effectively restricted others from using the code with competing products — a pattern Stallman considered incompatible with free software.

## The Three-Year Drafting Process

The GPL v3 drafting process (2004-2007) was the most public and participated-in license drafting in FOSS history. The FSF published four discussion drafts and solicited comments from the community, the FSF associate members, and interested parties including major corporations. The drafting committee included representatives from multiple constituencies.

The process was contentious. The anti-tivoization provisions (section 6 of GPL v3, requiring that installation information accompany hardware distributions) were strongly opposed by hardware manufacturers. The patent retaliation provisions were opposed by companies that considered software patent cross-licensing a necessary defensive practice.

## Key Provisions

GPL v3 addressed GPL v2's gaps in several ways:

- **Anti-tivoization (§6)**: Distributors of GPL v3 software in consumer devices must provide the "Installation Information" needed to install and run modified versions — not just the source code, but the keys, signatures, or other means needed to actually run a modified version.
- **Patent termination (§10-11)**: Contributors grant a patent license for their contributions; if a user initiates patent litigation against any party for the software, their license terminates.
- **Compatibility with Apache License 2.0**: GPL v3 was explicitly drafted to be compatible with the Apache License 2.0 (GPL v2 was not compatible), enabling code from Apache-licensed projects to be incorporated into GPL v3 projects.
- **Anti-DRM (§3)**: Makes explicit that GPL v3 does not permit distributing software under laws that restrict circumvention of digital locks (anti-circumvention provisions like DMCA §1201) in a way that would override the freedoms GPL v3 grants.

## Linux Kernel Stays on GPL v2

[[linus-torvalds]]'s decision to keep the Linux kernel on [[gpl-v2]] was significant and deliberate. Torvalds expressed skepticism about GPL v3's anti-tivoization provisions, arguing that he did not consider tivoization a problem — that a device manufacturer should be able to control what software runs on their hardware. He also criticized the patent provisions.

Because the Linux kernel is licensed under "GPL v2 only" (not "GPL v2 or later"), it cannot be upgraded to GPL v3 without consent from all contributors who hold copyright — a logistically impossible task given the thousands of contributors. The kernel's GPL v2 status is permanent absent a complete rewrite.

This created a situation where the FSF's flagship license and the Linux kernel — the most widely deployed free software — were legally incompatible (code licensed "GPL v3 only" cannot be combined with Linux kernel code). The divergence symbolized the broader split between the FSF's principled free software position and the pragmatic direction of the FOSS ecosystem.

## Adoption

GPL v3 adoption was significant but not universal. Many projects that had used GPL v2 with the "or later" clause upgraded to GPL v3 or AGPL. The GNU tools (GCC, GDB, etc.) moved to GPL v3. Bash, GMP, and many other GNU project components are GPL v3. But the Linux kernel, the most deployed GPL-licensed software, remained on GPL v2. Many projects chose permissive licenses instead, accelerating the [[mainstream-adoption-and-corporate-embrace-2005-2014]] trend toward Apache License 2.0 and MIT.
