---
id: linux-kernel-release-1991
title: "Linus Torvalds Releases Linux Kernel (1991)"
type: event
tags:
- linux
- kernel
- linus-torvalds
- gpl
- gnu
- usenet
importance: 9
date: 1991-08-25
location: "Helsinki, Finland"
participants:
- linus-torvalds
---

On August 25, 1991, [[linus-torvalds]] posted the following to the comp.os.minix Usenet newsgroup:

> "I'm doing a (free) operating system (just a hobby, won't be big and professional like gnu) for 386(486) AT clones."

This post — often called the "just a hobby" announcement — is the conventional date marker for the Linux kernel's public introduction, though the 0.01 release of the kernel itself followed in September 1991 and the first more widely distributed 0.02 release came shortly after. The date of the Usenet post is used here as the event date; the exact dates of the early kernel versions are documented but somewhat fluid.

## Context: The Missing Kernel

The timing was consequential. By 1991, the [[gnu-and-free-software-1983-1997]] era had produced a substantial free software toolkit: GCC, GDB, GNU Emacs, GNU Make, and the other GNU utilities. What the GNU Project had consistently lacked was a kernel. The GNU Hurd (GNU's own kernel project) was under development but technically ambitious and chronically delayed. GNU tools existed; a GNU operating system did not.

Torvalds had been using Minix — a small Unix-like system designed by Andrew Tanenbaum for teaching operating systems — and found its limitations frustrating. He began writing his own kernel for the Intel 386 processor while a computer science student at the University of Helsinki. The result was pragmatic rather than ideologically driven: Torvalds wanted a usable Unix-like environment, not to advance a philosophical position about software freedom.

## Licensing: The GPL Decision (1992)

The early Linux releases were not under the GPL. Version 0.01 used a custom license that explicitly prohibited commercial use. In 1992, Torvalds relicensed Linux under the [[gpl-v2]] — a decision he described as "one of the best things I ever did." The GPL v2 license meant that all modifications to the kernel would be required to be released as free software, preventing proprietary forks from diverging without contributing back.

Torvalds' decision to use GPL v2 rather than a permissive license was foundational for the Linux kernel's development model. The kernel has remained on GPL v2 (notably *not* upgrading to [[gpl-v3-release-2007]] when that was released in 2007 — a decision Torvalds made explicitly, over objections from [[richard-stallman]] and the FSF).

## Significance to the FOSS Movement

The Linux kernel release was the enabling event for GNU/Linux as a complete free operating system. Without a free kernel, the GNU Project's tools remained orphaned — dependent on proprietary kernels or on academic systems like BSD (which was under legal challenge). Linux completed the stack.

The development model that emerged — Torvalds accepting patches from a distributed, internet-coordinated community, integrating them with his own judgment — became the empirical basis for [[eric-raymond]]'s [[bazaar-model]] analysis in [[cathedral-and-the-bazaar-1997]]. The Linux kernel was Raymond's central case study, and it was Linux's success (not GNU's tooling, which predated the internet-scale coordination) that made the bazaar model legible as a general principle.

Linux also demonstrated that a project organized around volunteer contribution and meritocratic peer review could produce software competitive with — and eventually superior to — commercially developed systems. This demonstration was the empirical foundation for the open source rebranding of 1998: the [[foresight-open-source-meeting-1998]] and [[osi-founding-1998]] were predicated on Linux's visible success.

By the [[mainstream-adoption-and-corporate-embrace-2005-2014]] era, Linux was running the majority of servers on the internet, all of Android's devices, and most of the cloud computing infrastructure. The "just a hobby" post has not aged well as a prediction.
