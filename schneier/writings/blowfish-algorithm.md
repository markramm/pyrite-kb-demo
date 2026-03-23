---
id: blowfish-algorithm
title: "Blowfish: A Fast New Secret-Key Block Cipher"
type: writing
importance: 8
tags:
- cryptography
- algorithm
- cipher
- symmetric-key
- open-source
writing_type: algorithm
date: "1993-01-01"
publisher: "Fast Software Encryption Workshop, Cambridge"
key_concepts:
- schneiers-law
research_status: draft
---

Blowfish is a symmetric-key block cipher designed by Schneier and published in 1993 as a free, unpatented alternative to DES and other proprietary or patented ciphers. It was one of Schneier's most practically significant technical contributions and became one of the most widely deployed ciphers of the 1990s and 2000s, embedded in hundreds of software products and used in applications ranging from password hashing to file encryption.

## Technical Design

Blowfish operates on 64-bit blocks with a variable-length key from 32 to 448 bits. Its design is a Feistel network with 16 rounds and a key schedule that is deliberately expensive — it takes significant computation to set up the key, which makes brute-force key search expensive while keeping per-block encryption fast once the key is established. This expensive key setup is what makes Blowfish particularly effective as a password hashing foundation (later formalized in the bcrypt algorithm by Niels Provos and David Mazières, which uses Blowfish's key schedule directly).

The cipher's design philosophy reflects Schneier's values at the time: simplicity, public availability, conservatism in design, and openness to analysis. Blowfish was published with full specifications and encouraged cryptanalysis, consistent with [[schneiers-law]] — the argument that the security of a cipher can only be established through public expert analysis, not through the claims of its designer.

## The Open and Free Design

Blowfish was explicitly placed in the public domain. Schneier designed it in part as a response to what he saw as the problematic landscape of cipher availability: DES was too weak (56-bit key), triple-DES was slow, RSA's RC4 and RC5 were proprietary, and IDEA was patented (which complicated use in some contexts). Blowfish offered a fast, strong, unpatented, and unencumbered alternative.

This decision — to publish a strong cipher freely rather than patent it — was consistent with the cypherpunk ethos of the era and with Schneier's view that strong cryptography needed to be freely available to the public. It connects to the broader context of the [[crypto-wars-export-controls]] debate, in which the government's argument for controlling cryptography was undermined by the free availability of strong algorithms in academic publications and software.

## Adoption and Legacy

Blowfish was widely adopted in the 1990s and appeared in numerous commercial and open-source products. It became particularly important through bcrypt, which was adopted as the default password hashing scheme in OpenBSD and is now the dominant password hashing algorithm across web applications globally.

Schneier's own assessment has evolved: he has recommended that for new applications, designers prefer AES or other modern ciphers, noting that Blowfish's 64-bit block size creates birthday attack vulnerabilities in high-volume applications. His own [[twofish-algorithm]] — designed for the [[aes-competition]] in 1998 — was intended as the successor, addressing the block size limitation among other improvements.

## Relationship to Applied Cryptography

Blowfish was designed in 1993 and appeared in the first edition of [[applied-cryptography]] in 1994, which gave it immediate wide exposure. The book's massive circulation functioned as an accelerant for Blowfish adoption — engineers reading Applied Cryptography for the first time found a free, fully specified, well-analyzed cipher ready for implementation. The algorithm and the book were mutually reinforcing: the book gave Blowfish visibility, and Blowfish gave the book a practical, immediately usable original contribution.
