---
id: why-cryptography-is-harder-than-it-looks
title: "Why Cryptography Is Harder Than It Looks"
type: writing
importance: 6
tags:
- cryptography
- essay
- security
- implementation
writing_type: essay
date: "1997-01-01"
publisher: "Information Security Bulletin"
key_concepts:
- schneiers-law
- security-is-a-process
- security-mindset
research_status: draft
---

"Why Cryptography Is Harder Than It Looks" is an essay published by Schneier in 1997, in the period between the first and second editions of [[applied-cryptography]]. It addresses a gap that the success of Applied Cryptography had itself created: a large population of engineers who had read the book, understood the algorithms, and proceeded to implement cryptographic systems that were nevertheless insecure — because the hard part of cryptography is not the algorithms but the protocols, the implementation, and the threat model.

## The Argument

The essay makes the case that cryptographic security has three distinct layers, each capable of undermining the others:

First, the algorithm: is the cipher or protocol mathematically sound? This is the layer Applied Cryptography addresses most directly, and it is the layer that cryptography researchers have had the most success analyzing.

Second, the protocol: does the way the algorithm is used in context actually achieve the desired security property? Many protocols that use sound cryptographic primitives fail at this level — they are vulnerable to replay attacks, man-in-the-middle attacks, or other protocol-level failures that have nothing to do with the underlying mathematics.

Third, the implementation: does the actual code correctly instantiate the protocol? Implementation errors — side-channel vulnerabilities, buffer overflows, timing attacks, incorrect random number generation — break systems that are sound at the algorithm and protocol levels.

## [[schneiers-law]] Elaborated

The essay is one of the earliest detailed treatments of what would become [[schneiers-law]]. Schneier makes the argument that amateur cryptographers can always produce ciphers they themselves cannot break — but that the test of a cipher is whether professional cryptanalysts, given full knowledge of the algorithm and unlimited time, can find weaknesses. The same applies to protocols and implementations: the test is not whether the designer can see the flaw, but whether an expert adversary can find it.

This is an epistemological claim about security: you cannot prove a cryptographic system secure; you can only fail to find breaks despite serious effort. Security is therefore an inductive confidence built on the failure of expert attacks, not a deductive property proved from first principles. This has significant implications for the [[security-mindset]] — it means that security evaluation requires adversarial thinking and sustained expert scrutiny.

## Context and Audience

The essay was written for a professional security audience and assumes familiarity with basic cryptographic concepts. It reads as a practitioner's warning: here are the ways that competent engineers go wrong when implementing cryptographic systems. The specific failure modes it describes — rolling your own protocol, using a cipher without a MAC, misusing random number generators — were common at the time and remain common. The essay functions as a troubleshooting guide for the implementation of [[applied-cryptography]]'s lessons.

## Relationship to the Arc

This essay belongs to the [[cryptography-era]] but anticipates the [[security-thinking-pivot]]. It is Schneier beginning to see the limits of the algorithmic focus that Applied Cryptography exemplified, without yet having articulated the broader critique that [[secrets-and-lies]] would make. It is a step in the development of his thinking, visible in retrospect as an early sign of the direction he was heading.
