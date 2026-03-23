---
id: matt-blaze
title: "Matt Blaze"
type: person
tags:
- cryptography
- clipper-chip
- crypto-wars
- security-research
- policy
importance: 7
role: "Security researcher at AT&T Bell Labs / Penn, Clipper Chip cryptanalyst, wiretapping policy expert"
affiliations:
- electronic-frontier-foundation
research_status: draft
---

Matt Blaze is a security researcher who spent much of his career at AT&T Bell Labs (later AT&T Labs Research) before moving to the University of Pennsylvania. He is best known for two contributions: his 1994 paper demonstrating a fundamental flaw in the Clipper Chip's Law Enforcement Access Field (LEAF), which critically damaged the [[clipper-chip-announcement]] proposal, and his extensive research on wiretapping systems and their security vulnerabilities — work that anticipated the concerns later validated by the [[snowden-revelations]].

## The Clipper Chip Attack

The [[clipper-chip-announcement]] in 1993 proposed a government-backed encryption standard with a key escrow mechanism: a Law Enforcement Access Field (LEAF) in every encrypted message that would allow lawful wiretapping. The NSA claimed the LEAF mechanism was secure against tampering. Blaze analyzed it and found that a user could spoof the LEAF — construct a fake, valid-looking field while using a key not held in escrow — making the wiretapping mechanism defeatable by the very criminals it was supposed to catch.

This result was technically elegant and politically devastating. The government's argument for the Clipper Chip rested on the claim that it would allow lawful wiretapping without creating a general backdoor vulnerability. Blaze showed the mechanism would not even reliably enable the wiretapping it was designed for, while still creating all the security risks of a backdoor. It was exactly the kind of results that Schneier was simultaneously making at a systems level in [[applied-cryptography]] and in his broader writing — that security mechanisms designed to serve multiple masters tend to serve none of them well.

Schneier cited Blaze's result extensively and it became a canonical example in the [[crypto-wars-export-controls]] debates of why mandated backdoors are a bad idea technically, not just politically. The Clipper Chip attack demonstrated that the [[security-mindset]] — asking what can go wrong and how — would naturally uncover these flaws, and that the NSA had not applied that mindset to its own design.

## Wiretapping Research

Blaze's subsequent research on wiretapping systems was prescient. Working with colleagues including [[whitfield-diffie]], he examined the security properties of CALEA (the Communications Assistance for Law Enforcement Act) implementations and found that the lawful interception infrastructure being built into telephone systems created significant security vulnerabilities: interfaces that could be exploited by unauthorized parties, not just authorized law enforcement. A 2005 paper demonstrated that CALEA-compliant systems in Greece had been compromised and used to spy on Greek government officials — exactly the scenario the Clipper Chip critics had predicted.

This body of work intersects with Schneier's arguments in [[data-and-goliath]] and in his long-running commentary on the [[schneier-on-security-blog]]: surveillance infrastructure built for government use creates attack surfaces that adversaries will exploit. The security community's concerns about backdoors were not paranoid speculation but empirically grounded engineering judgment.

## Relationship to Schneier

Blaze and Schneier occupy parallel positions in the security community: both are technically rigorous researchers who engage seriously with policy, both were prominent critics of the Clipper Chip and key escrow, and both have a practice of communicating technical security arguments to policy audiences. Blaze's work is more narrowly focused on wiretapping and surveillance systems; Schneier's range is broader. But the Clipper Chip period brought them to the same fights, and Blaze's technical results provided exactly the kind of concrete empirical backing that Schneier's more sweeping arguments needed.

Blaze has continued to do important technical work on surveillance systems, wireless security, and physical security — including research on lock vulnerabilities that illustrates the same [[security-mindset]] principle Schneier articulates: experts see attacks that non-experts cannot imagine, because experts know how things actually work rather than how they are supposed to work.
