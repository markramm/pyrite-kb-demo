---
id: aes-competition
title: "AES Competition (1997–2000)"
type: event
importance: 8
tags:
- AES
- cryptography
- NIST
- Twofish
- Rijndael
- algorithm-competition
- cipher-design
date: "1997-01-01"
location: "United States"
participants:
- nist
- niels-ferguson
- john-kelsey
- ross-anderson
- whitfield-diffie
- daniel-bernstein
status: confirmed
---

The Advanced Encryption Standard (AES) competition was a public evaluation process run by [[nist]] from 1997 to 2000 to select a replacement for the aging Data Encryption Standard (DES). The competition was a landmark in cryptographic practice: it was open, international, and transparent, with all submitted algorithms published and subject to public cryptanalysis. Schneier co-designed Twofish, one of the five finalist algorithms, making the competition a direct expression of his [[cryptography-era]] work.

## Background: The DES Problem

DES, standardized in 1977, used a 56-bit key — a length that had been controversial at the time and was definitively inadequate by the mid-1990s. Brute-force attacks against 56-bit DES became feasible with specialized hardware, and DES's known structural properties made it vulnerable to differential and linear cryptanalysis. [[nist]] announced the AES competition in 1997 as a transparent, merit-based process to select a modern replacement.

The decision to run an open competition was itself significant: it rejected the closed, NSA-adjacent process that had produced DES in favor of public international evaluation. Schneier had argued in [[applied-cryptography]] that this kind of open analysis was the only reliable way to establish confidence in a cryptographic algorithm — the principle later formalized as [[schneiers-law]].

## Twofish

Schneier led the Twofish design team, which included [[niels-ferguson]], [[john-kelsey]], and several other researchers. Twofish was a 128-bit block cipher featuring a complex key schedule and a structure designed to resist all known attack methods. It was submitted to the competition in 1998 and selected as one of five finalists in 1999.

The design philosophy of Twofish reflected Schneier's cryptographic principles: conservative design choices, heavy emphasis on security margin over performance, and transparency about the design rationale. The team published extensive documentation and actively invited cryptanalysis throughout the competition.

## The Competition and Rijndael's Selection

The five finalists — Twofish, Rijndael (by Joan Daemen and Vincent Rijmen), Serpent, RC6, and MARS — underwent two additional years of public evaluation. [[nist]] selected Rijndael in October 2000, citing its combination of security, efficiency, and simplicity. Twofish was considered highly secure but was judged less efficient in software implementations across the range of target platforms.

Schneier accepted the outcome publicly and professionally. He wrote that Rijndael was a strong choice and that the competition itself — the open evaluation process — was as important as any single outcome. His post-competition writing analyzed the selection criteria and the tradeoffs between the finalists in terms accessible to practitioners, continuing the educational role he had established with [[applied-cryptography]].

## Significance for Schneier's Intellectual Development

The AES competition marked both a high point and a transition in Schneier's technical work. Twofish was his most sophisticated algorithmic design, produced by a well-organized team and subjected to the most rigorous public evaluation ever applied to a cipher. Its finalist status demonstrated the quality of Schneier's cryptographic work.

At the same time, the competition coincided precisely with the [[security-thinking-pivot]]: [[secrets-and-lies]] was published in the same year Rijndael was selected. The AES competition was the culmination of the [[cryptography-era]] — the final major technical project before Schneier redirected his attention from algorithm design to systems security. The competition's transparency and open evaluation model remained for him an exemplar of how to build confidence in security-critical systems: not through authority but through sustained public scrutiny.
