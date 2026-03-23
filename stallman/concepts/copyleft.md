---
id: copyleft
title: Copyleft
type: concept
tags:
- copyleft
- legal
- gpl
- licensing
- foundational
links:
- target: digital-rights-management-critique
  relation: related_to
  note: Copyleft and Doctorow's DRM critique share the core argument that technical
    restrictions on copying harm users and downstream creativity
  kb: doctorow
- target: adversarial-interoperability
  relation: related_to
  note: Copyleft and adversarial interoperability are complementary strategies against
    proprietary lock-in. Copyleft prevents code from being enclosed; adversarial interoperability
    breaks existing enclosures. Both use the existing legal system against its conventional
    operation.
  kb: doctorow
- target: hacking-as-systems-subversion
  relation: related_to
  note: Copyleft is a paradigmatic example of what Schneier calls hacking as systems
    subversion — using copyright law's own mechanisms against its conventional purpose.
    Both Stallman and Moglen have described copyleft as a 'legal hack.' Schneier's
    framework generalizes exactly this kind of rule-following intent-subversion.
  kb: schneier
- target: oscon-resignation
  relation: related_to
  note: Wardley's OSCON resignation was triggered by Canon's refusal to open-source
    Zimki under GPLv3 — the very license Stallman's copyleft philosophy produced.
    A concrete intersection of Wardley's strategic framework with Stallman's legal
    mechanism.
  kb: wardley
importance: 10
concept_type: legal
first_appeared: Emacs distribution terms, circa 1985; named and theorized in gnu-manifesto
  (1985)
key_writings:
- gnu-manifesto
- gpl-v1
- gpl-v2
- gpl-v3
- free-software-free-society
- why-software-should-be-free
related_concepts:
- four-freedoms
- gpl-copyleft-mechanism
- free-software-definition
- tivoization
- saas-loophole
- gnu-manifesto-concept
research_status: draft
---

Copyleft is [[stallman]]'s central legal innovation: using copyright law to guarantee freedom rather than restrict it. Where traditional copyright reserves all rights to the author, copyleft licenses grant broad permissions while attaching a condition — any distributed derivative work must be released under the same terms. The result is a license that is self-propagating: freedom, once granted, cannot be taken away by downstream recipients. [[stallman]] has situated copyleft within American political tradition in [[gpl-and-american-way]], connecting the reciprocal obligations it enforces to broader American ideals of liberty.

The name is a deliberate pun on "copyright" — the copyright symbol is rotated and the word reversed to signal that the legal mechanism is being used for the opposite of its conventional purpose. The pun originated in a Symbolics hacker culture context but was adopted by [[stallman]] as the name for his legal strategy.

## The Mechanism

Copyright gives authors exclusive rights over copying, distribution, and modification. A proprietary software vendor uses these rights to prevent users from sharing or studying the code. Copyleft uses the same rights differently: the author grants permission to copy, distribute, and modify — but only on the condition that all recipients receive the same permissions. Any attempt to distribute a modified version without extending these freedoms to recipients violates the license and therefore infringes copyright.

This is not a separate legal right; it is a condition attached to the exercise of copyright permissions. The legal mechanism is explained in detail under [[gpl-copyleft-mechanism]].

## Origin

The concept emerged from a practical problem [[stallman]] encountered at the [[mit-ai-lab]] in 1980: Symbolics Corporation had taken the MIT AI Lab's Lisp Machine software, improved it under a proprietary license, and was not required to share those improvements. Stallman could see their changes but could not legally incorporate them back. The experience made visceral the problem that copyleft was designed to solve.

The first implementation was the Emacs distribution terms (circa 1984–1985), which required anyone who distributed a modified Emacs to provide the source code. This predates the term "copyleft" and the formal GPL. The [[gnu-manifesto]] (1985) articulates the philosophical argument. The [[gpl-v1]] (1989) was the first formal, reusable copyleft license.

## Strong and Weak Copyleft

Copyleft exists on a spectrum:

**Strong copyleft** (the [[gpl-v2]], [[gpl-v3]]): Any program that incorporates GPL code and is distributed must itself be GPL-licensed. This is the "viral" property that makes the GPL controversial in commercial contexts.

**Weak copyleft** (the [[lgpl]]): Modifications to the licensed library must be shared, but programs that merely link to the library can be distributed under different terms. Designed for libraries where [[stallman]] judged that broader adoption outweighed the strategic cost of permitting proprietary use.

**Network copyleft** (the [[agpl]]): Extends the trigger to include network use, closing the [[saas-loophole]] in GPLv2.

## The "Viral" Characterization

Critics — particularly in commercial and open source communities — describe copyleft as "viral" because GPL code, once included in a program, requires the entire program to be GPL-licensed if distributed. [[stallman]] rejects this framing as a rhetorical attack: the condition only applies when you choose to distribute, and it applies only to the terms of distribution. No one is forced to distribute GPL software.

The viral characterization has had real strategic consequences: many corporations avoided GPL code for years (and some still do), preferring permissive licenses like MIT or Apache. [[stallman]] regards this as an intended feature — copyleft is a barrier against appropriation, not a bug.

## Copyleft as Legal Hack

[[stallman]] and [[eben-moglen]] have both described copyleft as a "hack" on copyright — using the legal system against its own normal operation. [[eben-moglen]] refined this characterization in his legal scholarship on the GPL. The note [[copyleft-as-legal-hack]] explores this framing in depth.

## Influence Beyond Software

Copyleft's logic influenced [[larry-lessig]]'s [[creative-commons]] project, particularly the ShareAlike licenses. The [[free-software-foundation]] has consistently argued that the ShareAlike principle is sound but that Creative Commons licenses are not appropriate for software. The Wikipedia use of CC BY-SA is a direct descendant of copyleft thinking applied to encyclopedic content.

Copyleft remains the most debated element of [[stallman]]'s legacy. Its defenders argue it is the only mechanism that prevents freedom from being extinguished by accumulation of proprietary derivatives. Its critics argue that permissive licenses achieve broader adoption and therefore more freedom in practice. [[stallman]] regards this as a confusion of freedom with convenience — the strategic core of [[software-freedom-vs-open-source]].
