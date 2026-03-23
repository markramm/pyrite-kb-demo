---
id: skein-hash-function
title: "Skein Hash Function"
type: writing
importance: 7
tags:
- cryptography
- hash-function
- algorithm
- nist
- sha-3
writing_type: algorithm
date: "2008-01-01"
publisher: "NIST SHA-3 Competition Submission"
coauthors:
- niels-ferguson
- john-kelsey
key_concepts:
- schneiers-law
research_status: draft
---

Skein is a cryptographic hash function designed by Schneier and collaborators and submitted to the NIST SHA-3 hash function competition in 2008. Like [[twofish-algorithm]] in the AES competition, Skein was a finalist — one of five algorithms selected for the final round of the SHA-3 competition — and like Twofish, it was ultimately not selected. NIST chose Keccak (now SHA-3) in 2012. Skein nonetheless represents a significant cryptographic contribution and was widely analyzed during the competition process.

## Technical Design

Skein is built on the Threefish block cipher, designed specifically as Skein's core component. Threefish is a large-block cipher — with 256, 512, or 1024-bit block sizes — designed for software efficiency and simplicity of analysis. Skein wraps Threefish in the Unique Block Iteration (UBI) chaining mode to construct a hash function, and adds a configuration mechanism that allows Skein to support a wide range of output sizes and use cases (standard hashing, tree hashing, message authentication, key derivation, and others) from a single design.

The co-designers included [[niels-ferguson]], [[john-kelsey]], and other members of the Twofish team, reflecting the continuity of Schneier's cryptographic collaborations across the AES and SHA-3 competition periods.

## The SHA-3 Competition Context

The SHA-3 competition was launched by [[nist]] in response to theoretical weaknesses found in the SHA-1 and MD5 hash functions. It followed the model of the [[aes-competition]] — open, public, with extended community cryptanalysis — which both Schneier and the broader community regarded as the right model for standardization. Schneier participated as both a designer (submitting Skein) and a commentator (writing extensively on the competition process on [[schneier-on-security-blog]]).

The competition attracted 64 initial submissions, which were narrowed to 14 second-round candidates and then 5 finalists. Skein's selection as a finalist represented validation of its design quality. Its non-selection reflected NIST's judgment that Keccak had better overall properties, particularly its use of a sponge construction that was architecturally distinct from SHA-2 and offered different security assumptions.

## The Team and the Schneier Cryptographic Network

Skein illustrates the collaborative structure of Schneier's cryptographic work. He has never worked as a solo designer; his cryptographic contributions are consistently team efforts. The recurring collaboration with [[niels-ferguson]] (co-designer of Twofish and co-author of [[practical-cryptography]]) and [[john-kelsey]] (co-designer of Twofish) represents a sustained working relationship across multiple major cryptographic projects. This network of cryptographic collaborators is characteristic of the [[counterpane-internet-security]] and post-Counterpane period.

## Legacy

Skein and Threefish are available in open-source implementations and are used in various applications, though not as a major standard (Keccak/SHA-3 holds that role). The Skein competition submission document — a technical specification of the algorithm with full security analysis — is itself a substantial piece of cryptographic writing, notable for the clarity and depth of its security arguments.

Like Twofish, Skein's significance in Schneier's arc is partly as evidence of sustained cryptographic seriousness through his transition from pure cryptographer to public intellectual. Even as Schneier was writing [[data-and-goliath]] and [[click-here-to-kill-everybody]], he was also designing hash functions for international cryptographic competitions. The two modes of work — technical contribution and public commentary — coexisted throughout his career.
