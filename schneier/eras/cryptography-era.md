---
id: cryptography-era
title: "Cryptography Era (1988–2000)"
type: era
importance: 9
tags:
- cryptography
- algorithms
- crypto-wars
- foundational
- blowfish
- twofish
date_range: "1988-2000"
key_writings:
- applied-cryptography
- e-mail-security
- blowfish-algorithm
- twofish-algorithm
- practical-cryptography
key_concepts:
- security-is-a-process
- schneiers-law
- attack-trees
affiliations:
- counterpane-internet-security
---

The cryptography era spans Schneier's emergence as a working cryptographer and security engineer through the publication of [[applied-cryptography]] and the design of foundational ciphers. This is the period in which Schneier built his technical reputation: as an algorithm designer, a synthesizer of cryptographic knowledge, and a voice in the Crypto Wars policy battles that set the terms for civilian use of strong cryptography.

## Early work and the applied cryptography project

Schneier entered the security field in the late 1980s, working as a cryptographer and systems engineer. His early writing reflected the conviction that the technical problem — getting strong cryptography into the hands of practitioners — was the central challenge. [[e-mail-security]] (1995) was an early practical guide to applying cryptographic tools to electronic mail, and [[protect-your-macintosh]] (1994) addressed computer security for personal users — both reflecting the same mission of making security accessible. The result was [[applied-cryptography]], published in 1994, which arrived at the precise moment when the early commercial internet was generating demand for cryptographic tools that engineers could actually implement. The [[applied-cryptography-publication]] event marked a turning point: the book's release coincided with the peak of the Crypto Wars policy battles and made Schneier a central figure in the debate over civilian access to strong cryptography.

The book was encyclopedic and deliberately practical: C source code was included, export-control implications were acknowledged and pushed against, and Schneier treated cryptography as a craft to be practiced, not a theoretical discipline to be contemplated. For a generation of engineers, [[applied-cryptography]] was the first complete technical map of a previously scattered field.

## Algorithm design

Alongside the book project, Schneier was designing ciphers. [[blowfish-algorithm]] (1993) was a fast, unpatented, public-domain block cipher designed as an alternative to DES, which was already showing its age against brute-force attacks. Blowfish was widely adopted in commercial and open-source software, including password hashing systems (bcrypt). [[twofish-algorithm]] followed as a more sophisticated design submitted to the [[aes-competition]] launched by [[nist]] in 1997. Schneier co-designed Twofish with [[niels-ferguson]], [[john-kelsey]], and others; the cipher was a finalist but ultimately lost to Rijndael in 2000. The deep cryptographic collaboration with Ferguson also produced [[cryptography-engineering]], the successor to [[practical-cryptography]] that became the definitive practitioner's guide to applied cryptographic engineering.

The algorithm design work gave Schneier's writing credibility it could not have achieved from commentary alone. He was not merely explaining other people's cryptography — he was producing it, having it analyzed by the community, and refining it through the public evaluation process.

## The Crypto Wars context

The [[crypto-wars-export-controls]] battle ran through this entire period. ITAR classified strong cryptographic software as a munition, limiting export and complicating civilian deployment. The [[clipper-chip-announcement]] in 1993 brought the conflict to a head: the NSA-designed Clipper Chip offered encryption with a built-in key escrow backdoor, and the Clinton administration sought to make it the standard for civilian voice communications. Schneier's consistent position was that key escrow was technically unworkable and that the underlying premise — government should control civilian access to cryptography — was wrong.

This brought him into the orbit of [[phil-zimmermann]] (then defending PGP against export-control prosecution), [[whitfield-diffie]] (public-key pioneer and key escrow opponent), and the broader cypherpunk community that included [[john-gilmore]], [[tim-may]], and [[eric-hughes]]. Schneier was not a founding cypherpunk but was intellectually adjacent: he shared their technical commitments and their policy conclusions, even if he came to them through engineering rather than libertarian ideology.

## The limit of the technical frame

By the late 1990s, Schneier was beginning to sense the limits of the framing that had produced [[applied-cryptography]]. Systems that used correct cryptographic primitives were still failing in practice — not because the math was wrong but because the systems were deployed in environments full of human and organizational complexity that cryptographic correctness could not address. This intuition crystallized into [[secrets-and-lies]] (2000), which publicly repudiated the implicit worldview of [[applied-cryptography]] and marked the transition to the [[security-thinking-pivot]].

The cryptography era ended not with failure but with a recognition that Schneier's own most successful work had been, in his retrospective judgment, misleading — that it had inadvertently reinforced the idea that the right algorithm could make a system secure, when the harder truth was that no algorithm could substitute for systematic security thinking.
