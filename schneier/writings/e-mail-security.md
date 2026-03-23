---
id: e-mail-security
title: "E-Mail Security: How to Keep Your Electronic Messages Private"
type: writing
importance: 5
tags:
- email
- privacy
- cryptography
- pgp
- practical
writing_type: book
date: "1995-01-01"
publisher: "John Wiley & Sons"
key_concepts:
- schneiers-law
research_status: draft
---

E-Mail Security, published in 1995, is Schneier's practical guide to securing electronic mail, focused on the technologies then available: PGP (Pretty Good Privacy), PEM (Privacy Enhanced Mail), and S/MIME. It is a technical guide in the tradition of [[applied-cryptography]] — focused on helping practitioners implement specific security measures — rather than an analytical work. In Schneier's arc, it is a supporting work of the [[cryptography-era]], demonstrating the range of practical applications his technical writing addressed in the mid-1990s.

## Context and Purpose

In 1995, email security was an active concern for technically sophisticated users: the growth of the commercial internet was making email ubiquitous, but the default state of email was plaintext, readable to any server operator or network observer along its route. Cryptographic tools for email existed — [[phil-zimmermann]] had released PGP in 1991 — but their use was non-trivial and documentation was scattered.

E-Mail Security served as the accessible guide to using these tools. Its publication by Wiley connected it to the [[applied-cryptography]] readership and positioned Schneier as the practical implementation guide for the cryptographic concepts his larger book addressed more theoretically.

## PGP and the Crypto Wars Context

The book's treatment of PGP was significant in the context of the [[crypto-wars-export-controls]] debate. PGP had made [[phil-zimmermann]] the subject of a federal criminal investigation (eventually dropped) for allegedly violating export controls by making strong encryption available outside the United States. E-Mail Security was part of the broader effort to make strong cryptographic tools usable and understood, effectively extending the practical reach of free cryptography regardless of export regulations.

Schneier's relationship with Zimmermann and the broader cypherpunk community — which included [[tim-may]], [[eric-hughes]], [[john-gilmore]], and [[john-perry-barlow]] — was shaped in part by this shared commitment to the practical availability of strong cryptography for ordinary users.

## Position in the Arc

E-Mail Security is not among Schneier's most significant works. It is a practitioner's guide to a specific set of technologies at a specific moment, and the technologies it covers have been superseded (PGP remains in use but S/MIME and PEM have evolved significantly). Its significance is historical: it documents the state of email security in 1995 and reflects the period when cryptographic tools were moving from academic and activist circles to practical commercial use.

The book predates the [[security-thinking-pivot]] of [[secrets-and-lies]] and belongs entirely to the [[cryptography-era]] mode: here are the tools, here is how to use them, here is why the mathematics works. The human, organizational, and adversarial analysis that would come to characterize Schneier's later work is largely absent.
