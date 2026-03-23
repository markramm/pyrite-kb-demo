---
id: tivoization
title: Tivoization
type: concept
tags:
- tivoization
- hardware
- gplv3
- user-freedom
- technical
links:
- target: right-to-repair
  relation: related_to
  note: Tivoization and right-to-repair address the same structural problem from different
    legal traditions. Stallman identified that hardware cryptographic signing defeats
    software freedom; Doctorow addresses the same lock-in through consumer rights
    and antitrust frameworks.
  kb: doctorow
importance: 8
concept_type: technical
first_appeared: GPLv3 drafting process, 2006-2007
key_writings:
- gpl-v3
- free-software-free-society
- can-you-trust-your-computer
related_concepts:
- gpl-copyleft-mechanism
- copyleft
- four-freedoms
- digital-restrictions-management
- free-software-definition
research_status: draft
---

Tivoization names a practice that [[stallman]] identified during the [[gpl-v3]] drafting process: a hardware manufacturer ships a device running GPL-licensed software but uses cryptographic signing to prevent users from running modified versions of that software on the device. The name comes from TiVo, the digital video recorder company, which used this approach with its Linux-based devices in the early 2000s.

## The Problem

TiVo's hardware ran the Linux kernel (licensed under [[gpl-v2]]) and other GPL-licensed software. TiVo distributed the source code, as GPLv2 requires. But the hardware was designed to verify a cryptographic signature on all software before execution: it would only boot software signed with TiVo's private key. Users who compiled modified versions of the kernel from TiVo's published source would find their modifications refused by the hardware.

This satisfied the letter of GPLv2 — source code was available, users could technically modify it — but violated its spirit. [[stallman]]'s argument is that Freedoms 1 and 3 ([[four-freedoms]]) require not just the legal right to modify software but the practical ability to run those modifications. A user who can modify the source code but cannot run the result on their own device does not have meaningful freedom.

## The Mechanism of Restriction

Tivoization combines two independent layers of control:

1. **Software layer**: GPL source code is provided, satisfying the distribution requirement.
2. **Hardware layer**: Cryptographic signing prevents unsigned software from executing. The private key is held exclusively by the manufacturer.

The hardware restriction is not a copyright mechanism — it operates entirely outside the GPL's legal scope. This is what made tivoization invisible to GPLv2: the license could not reach hardware design choices.

## GPLv3's Response

Section 6 of [[gpl-v3]] addresses tivoization directly. For "user products" — consumer devices — distributors must provide "Installation Information": the cryptographic keys, signing certificates, or other information necessary to install modified software on the specific device. Without Installation Information, providing source code does not satisfy the GPL's requirements.

The definition of "user product" matters here: it covers devices primarily used by consumers (phones, DVRs, routers) rather than general-purpose servers or workstations. The FSF judged that consumer devices are where tivoization was most harmful — they are single-purpose devices where the user cannot simply install a different operating system.

## The Linus Torvalds Disagreement

Tivoization was the central point of dispute between [[stallman]] and [[linus-torvalds]] during the GPLv3 drafting process. Torvalds explicitly stated that he found tivoization acceptable and did not consider hardware restrictions a violation of the GPL's principles. He kept the Linux kernel under GPLv2 (with the "or later" clause removed), meaning it is not covered by GPLv3's anti-tivoization provisions.

This disagreement reflects a deeper philosophical difference: Torvalds prioritizes broad adoption and technical collaboration; [[stallman]] prioritizes user freedom. For Stallman, a device you cannot modify is a device that controls you — regardless of whether its software is technically "open source." The split is part of the broader [[software-freedom-vs-open-source]] division.

## Tivoization and Secure Boot

The concept has new relevance in the context of UEFI Secure Boot, which some PC manufacturers implement in ways that prevent users from installing alternative operating systems. [[stallman]] and the [[free-software-foundation]] have campaigned against Secure Boot implementations that lock out user-chosen software, treating them as a form of tivoization applied to general-purpose computers.

The [[digital-restrictions-management]] concept overlaps with tivoization: both use technical means to prevent users from exercising freedoms they might otherwise have. Tivoization focuses on the running of modified software; DRM focuses more broadly on the use and copying of content. But they share the same structure — a technical restriction that makes legal freedoms practically inaccessible.
