---
id: clipper-chip-announcement
title: "Clipper Chip Announcement"
type: event
importance: 9
tags:
- crypto-wars
- key-escrow
- NSA
- Clinton-administration
- government-surveillance
- backdoor
date: "1993-04-16"
location: "Washington, D.C."
participants:
- nsa
- phil-zimmermann
- whitfield-diffie
- dorothy-denning
- matt-blaze
status: confirmed
---

On April 16, 1993, the Clinton administration announced the Clipper Chip initiative: a hardware encryption chip for voice communications that included a key escrow mechanism allowing law enforcement to decrypt any protected conversation with a court order. The announcement launched the most intense phase of the [[crypto-wars-export-controls]] debates and became the defining confrontation over whether government could control civilian access to strong cryptography.

## The Technical Design

The Clipper Chip used the classified Skipjack algorithm, designed by the [[nsa]], to encrypt voice communications. The key escrow system split each chip's unique key into two components, held by two separate government agencies (initially the Treasury Department and NIST). Law enforcement agencies could obtain both components via court order to decrypt any Clipper-protected communication. The administration proposed Clipper as the standard for civilian and eventually commercial encryption.

The design's fundamental flaw — beyond the policy objections — was identified in the research community almost immediately. [[matt-blaze]] published a technical analysis in 1994 demonstrating a protocol vulnerability in the Law Enforcement Access Field (LEAF), the mechanism that transmitted the escrowed key information. The vulnerability allowed a user to bypass the key escrow entirely without disrupting the encrypted call, effectively defeating the purpose of the system while retaining its restrictions. This finding devastated the technical credibility of Clipper and accelerated its collapse.

## Schneier's Response

For Schneier, the Clipper Chip crystallized the argument he had been developing about the relationship between cryptography and policy. During the [[cryptography-era]], Schneier's position was straightforwardly technical: strong cryptography needed to be publicly available, freely implementable, and not encumbered by backdoors, because backdoors are vulnerabilities. Clipper's key escrow was not a policy accommodation but a cryptographic weakness: any system that can be decrypted by a third party under some circumstances can potentially be decrypted by adversaries who obtain those same keys or exploit the escrow mechanism.

Schneier's [[schneier-on-security-blog]] and [[crypto-gram-newsletter]] writings in subsequent years returned repeatedly to the Clipper episode as the template for evaluating all subsequent key escrow and lawful access proposals. The argument never changed: the technical analysis shows that backdoors are not a policy choice between privacy and security but a choice to weaken security everywhere in exchange for law enforcement convenience.

## The Broader Debate

The Clipper announcement galvanized the cryptographic community and the emerging digital rights movement. [[phil-zimmermann]] had already released PGP — and was under federal investigation for export violations — when Clipper was announced. [[whitfield-diffie]], whose public-key work had made civilian encryption technically feasible, became a prominent critic. [[dorothy-denning]], a prominent computer scientist, was among the few academic voices who argued publicly for key escrow, leading to high-profile debates with Schneier and others.

The [[electronic-frontier-foundation]] organized much of the opposition, providing legal resources, policy expertise, and public communication. The Clipper battle was in many ways the founding controversy of the digital rights movement: it established that technical decisions about cryptography were simultaneously political decisions about civil liberties, and that the security research community had a responsibility to participate in those political decisions.

## Outcome and Legacy

The Clipper Chip initiative collapsed by the mid-1990s under the combined weight of technical criticism, commercial opposition, and political resistance. Key escrow proposals returned repeatedly — in the FBI's Freeh-era "Going Dark" debates, in post-9/11 surveillance policy, and in the Apple-FBI iPhone encryption controversy of 2016 — and Schneier analyzed each iteration using the same framework he developed in response to Clipper. The [[clipper-chip-announcement]] set the terms of a debate that has not been resolved and defines the context of Schneier's policy work from the [[cryptography-era]] forward.
