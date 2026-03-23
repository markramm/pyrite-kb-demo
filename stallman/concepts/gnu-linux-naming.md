---
id: gnu-linux-naming
title: 'GNU/Linux: The Naming Argument'
type: concept
tags:
- gnu-linux
- naming
- credit
- philosophy
- rhetorical
importance: 7
concept_type: rhetorical
first_appeared: Stallman began insisting on 'GNU/Linux' after Linux kernel adoption
  circa 1992-1993
key_writings:
- free-software-free-society
- gnu-manifesto
- why-open-source-misses-the-point
related_concepts:
- software-freedom-vs-open-source
- four-freedoms
- gnu-manifesto-concept
- hacker-ethic-mit
- free-software-definition
research_status: draft
---

[[stallman]]'s insistence that the GNU/Linux operating system be referred to as "GNU/Linux" rather than simply "Linux" is one of his most publicly visible and contested positions. To many observers it appears as a petty dispute over credit. [[stallman]]'s argument is that it is about something more important: the visibility and survival of the free software philosophy.

## The Historical Claim

The factual basis of Stallman's position is not seriously disputed: when [[linus-torvalds]] released the Linux kernel in 1991, the rest of the operating system he used was largely the GNU system — the GNU C compiler, GNU C library, Bash shell, GNU coreutils, and other GNU components. The Linux kernel filled the one major gap in the GNU system (a kernel). The combination of the GNU system and the Linux kernel produced a complete, functional free operating system.

[[stallman]] argues that calling this system simply "Linux" — as has become standard — attributes the entire operating system to the kernel, which is a small (if critical) component. The [[gnu-project]] had spent ten years building the surrounding system; crediting only the kernel erases that work.

## Why Credit Matters

[[stallman]]'s argument is not primarily about personal credit (though he does not deny that credit matters). It is about what the name communicates about the nature and history of the system:

1. **Philosophical lineage**: "GNU/Linux" signals that the system is a product of the [[free-software-foundation]] and GNU Project's philosophy, not merely a technical collaborative effort. Calling it "Linux" severs this philosophical lineage.

2. **Movement visibility**: The [[gnu-project]] was founded on a specific ethical commitment — the [[four-freedoms]], [[copyleft]], user rights. "Linux" has become associated with the open source movement (see [[software-freedom-vs-open-source]]), which does not share all of these commitments. The name change, in Stallman's view, contributed to the marginalization of the free software philosophy within the community that uses free software.

3. **Practical consequences**: Users who know they are running GNU/Linux know to look to the GNU Project and FSF for guidance on software freedom. Users who think they are running "Linux" may not know there is a philosophical tradition behind the system that distinguishes free software from mere open source.

## Torvalds's Position

[[linus-torvalds]] has consistently declined to adopt the "GNU/Linux" name and has been dismissive of Stallman's argument. His position is pragmatic: "Linux" is the name people use, it has become a brand, and insisting on the longer name is pedantic. Torvalds does not share Stallman's philosophical commitments to the same degree — he has described the GPL as a good license for practical reasons (ensuring code is shared back) rather than ethical ones.

## The Hurd Factor

There is a counterfactual that complicates the historical argument: [[stallman]] spent enormous effort on the GNU Hurd microkernel, which was intended to be the kernel of the GNU system. The Hurd was never completed in a form suitable for production use. Linux succeeded where the Hurd did not. Some critics argue that Stallman's insistence on "GNU/Linux" is partly a response to the Hurd's failure — a way to claim credit for the success of a system that succeeded partly because it used a non-GNU kernel.

[[stallman]] acknowledges the irony but maintains the historical argument: whatever happened with the Hurd, the system that runs on Linux kernels is still predominantly the GNU system, and the name should reflect that. [[alexandre-oliva]]'s GNU Linux-libre project — which removes nonfree firmware blobs from the Linux kernel — is a practical extension of this position: if the kernel is to be part of the GNU system, it should meet the [[free-software-definition]].

## Cultural Impact

The naming dispute has become a cultural touchstone — a shorthand for the tension between Stallman's philosophical rigor and what critics see as his rigidity. Many people who are broadly sympathetic to free software find the GNU/Linux insistence tiresome. [[stallman]] has accepted this cost, treating it as evidence that the philosophical point is important enough to be worth making repeatedly even at the expense of his reputation.

The dispute is inseparable from the broader [[software-freedom-vs-open-source]] schism: it is both a symptom of and a contribution to the cultural separation between the free software community centered on the FSF and the open source community centered on the OSI and Linux kernel development.
