---
id: twofish-algorithm
title: "Twofish: A 128-Bit Block Cipher"
type: writing
importance: 8
tags:
- cryptography
- algorithm
- cipher
- aes
- symmetric-key
writing_type: algorithm
date: "1998-01-01"
publisher: "NIST AES Submission"
coauthors:
- niels-ferguson
- john-kelsey
key_concepts:
- schneiers-law
research_status: draft
---

Twofish is a symmetric-key block cipher submitted by Schneier and colleagues to the [[nist]] Advanced Encryption Standard competition in 1998. It was one of five finalists in the [[aes-competition]] — one of the most scrutinized cryptographic competitions in history — and while ultimately not selected as the AES (Rijndael was chosen in October 2000), Twofish is considered one of the strongest ciphers ever designed and is still widely used.

## Design and Technical Features

Twofish operates on 128-bit blocks with key sizes of 128, 192, or 256 bits. It is a 16-round Feistel network with a complex key schedule and uses MDS matrices, key-dependent S-boxes, and a PHT (pseudo-Hadamard transform) construction. The design was developed by Schneier, [[niels-ferguson]], [[john-kelsey]], [[david-wagner]], and Chris Hall — a team that included several of the most capable cryptographers of the era.

Twofish addressed the main limitation of [[blowfish-algorithm]]: it uses 128-bit blocks (matching the AES requirement) and was designed from the ground up to resist known attack techniques. The key-dependent S-boxes are a distinctive design feature — the S-boxes are constructed from the key itself, meaning the cipher's internal structure varies per key, which complicates differential and linear cryptanalysis.

## The AES Competition

The [[aes-competition]] was notable for its openness and rigor. NIST invited public submission of cipher designs and subjected all submissions to several years of public cryptanalysis before selecting a winner. This process was itself an expression of [[schneiers-law]] — the principle that the security of a cipher can only be established through expert public analysis, not through the designer's own assessment.

Twofish survived the public analysis phase without significant cryptographic weaknesses. Its non-selection was based on implementation efficiency considerations, not on cryptographic weakness. Rijndael (AES) was judged better suited for efficient implementation across a wider range of hardware and software environments, particularly constrained devices. Twofish remains unbroken as of 2026.

## Co-Design and the Counterpane Connection

Twofish was a team effort produced partly through [[counterpane-internet-security]], Schneier's consulting firm. The co-designers — particularly [[niels-ferguson]] and [[john-kelsey]] — were among Schneier's key intellectual collaborators throughout this period. Their collaboration would continue in the Skein hash function (see [[skein-hash-function]]) and in [[practical-cryptography]], a technical successor to [[applied-cryptography]] written with Ferguson.

## Legacy

Although Twofish was not selected as AES, it remains in widespread use. It is available in TrueCrypt and its descendants (VeraCrypt), in the GNU Privacy Guard, and in various other security products. Its status as an AES finalist means it has received more independent cryptanalytic scrutiny than almost any other cipher in existence, and it has emerged from that scrutiny without practical breaks.

Schneier has described the AES competition process itself — regardless of outcome — as a successful model for how cryptographic standards should be developed: publicly, with open competition, with extended community analysis, and with transparent criteria. The process vindicated the principles of open cryptographic development that [[applied-cryptography]] had helped establish.
