---
id: gpl-v2
title: "GNU General Public License version 2"
type: license
importance: 8
license_type: copyleft-strong
author: "Richard Stallman / Free Software Foundation"
date: 1991-06-01
spdx_id: "GPL-2.0-only"
key_provisions:
- "Copyleft: any derivative work distributed must use the same license"
- "Source code must be provided or offered when distributing binaries"
- "Section 7 'liberty or death' clause: if conditions prevent GPL compliance, do not distribute"
- "No additional restrictions beyond GPL terms"
related_licenses:
- gpl-v3
- lgpl
- agpl
tags:
- copyleft
- stallman
- fsf
- linux
- foundational-license
research_status: draft
---

The most widely deployed copyleft license in history and the license under which the Linux kernel is distributed. [[richard-stallman]] and the [[free-software-foundation]] published GPL v2 in June 1991, replacing the GPL v1 of February 1989. The earlier [[gpl-v3]] link reads backwards in time — v2 preceded v3 by sixteen years.

## What Problem It Solves

The GPL v2 solved the problem that [[copyleft]] — the principle that software freedom must be preserved through distribution — needed a legally robust mechanism. Earlier FOSS licenses either permitted proprietary relicensing (permissive licenses like [[mit-license]] and [[bsd-license]]) or had deficiencies that made them difficult to enforce.

The core mechanism: if you distribute software under GPL v2, you must provide the source code or a written offer to provide it, and any derivative works you distribute must also be under GPL v2. This creates the "viral" effect that distinguishes strong copyleft from permissive licensing — the license propagates forward through the supply chain of derivative works.

## The "Liberty or Death" Clause

Section 7 is named for Patrick Henry's "give me liberty or give me death" in movement lore. It states that if any condition (a patent license, a court order, anything) prevents you from fully complying with the GPL, then you may not distribute the software at all. The clause addresses the scenario where an entity tries to distribute GPL software while imposing additional restrictions through other legal mechanisms. You cannot have it both ways: either distribute freely or not at all.

## Linux and GPL v2

The [[linux-kernel-release-1991]] was originally released under a restrictive license that prohibited commercial use; Torvalds relicensed it to GPL v2 in 1992. This decision was historically decisive. The GPL v2 required that anyone distributing modified Linux kernels release those modifications — which meant that hardware vendors, distributors, and commercial users who built on Linux were forced into a commons-based relationship with the kernel development community.

When [[gpl-v3]] was released in 2007 ([[gpl-v3-release-2007]]), Torvalds and other kernel maintainers chose to remain on GPL v2 specifically ("GPL-2.0-only" rather than "GPL-2.0-or-later"). This decision reflects both principled disagreements with GPLv3 provisions and practical inertia — migrating a project with thousands of contributors would require assent from all copyright holders.

## The GPL v2 vs. Permissive Debate

GPL v2 sits at the center of the [[software-freedom-vs-open-source]] debate. From the free software perspective, permissive licenses fail to protect user freedom — they allow proprietary derivative works that deny downstream users the freedoms the original authors intended. From the open source pragmatist perspective, GPL v2's restrictions limit adoption, especially by corporations who cannot accept the copyleft conditions.

The [[lgpl]] was created as a compromise, allowing proprietary code to link against LGPL-licensed libraries without triggering copyleft. The [[apache-license-2]] addressed corporate adoption concerns differently, via explicit patent grants. The [[agpl]] addressed GPL v2's network-use gap.

GPL v2 remains in wide deployment: Linux, BusyBox, and many embedded systems tools operate under it. Its enforcement history — through the Software Freedom Conservancy and individual copyright holders — is the primary body of copyleft case law.
