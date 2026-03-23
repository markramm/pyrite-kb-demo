---
id: crypto-wars-export-controls
title: "Crypto Wars: Export Controls on Cryptography"
type: event
tags:
- crypto-wars
- ITAR
- export-controls
- civil-liberties
- NSA
- cypherpunks
- free-speech
links:
- target: adversarial-interoperability
  relation: related_to
  note: 'Crypto Wars were early adversarial interoperability: cypherpunks using mathematics to make surveillance technically infeasible. Doctorow generalizes the same move to platform competition'
  kb: doctorow
- target: software-patents-opposition
  relation: related_to
  note: Both are instances of legal/regulatory regimes restricting who can implement or distribute technical knowledge
  kb: stallman
importance: 9
date: "1993-01-01"
location: "United States"
participants:
- nsa
- ietf
- electronic-frontier-foundation
- phil-zimmermann
- whitfield-diffie
- john-gilmore
- tim-may
- eric-hughes
- daniel-bernstein
---

The Crypto Wars refers to the sustained policy conflict of the 1990s over the U.S. government's attempt to maintain control over civilian access to strong cryptography. Under the International Traffic in Arms Regulations (ITAR), encryption software was classified as a munition, restricting its export in the same category as weapons. This classification made it legally precarious to publish or distribute strong cryptographic code abroad — and, by practical extension, difficult to deploy it in internationally distributed software.

## ITAR and the Munitions Classification

The underlying legal framework dated to the Cold War. Cryptography had been an exclusively military and intelligence capability, and ITAR's munitions classification reflected that history. By the early 1990s, the classification was increasingly anachronistic: cryptographic theory was published in academic journals, algorithms like RSA were described in textbooks, and the growth of the internet made the concept of restricting the export of mathematical knowledge to physical borders operationally absurd.

[[nsa]] was the primary institutional defender of the export regime, motivated by the concern that widespread availability of strong cryptography would compromise signals intelligence collection. The agency's position was that export restrictions, combined with domestic key escrow proposals like the [[clipper-chip-announcement]], could preserve some version of lawful access as cryptography became commercially widespread. Within the academic community, [[dorothy-denning]] was the most prominent researcher who argued publicly in favor of key escrow and lawful access frameworks, providing a technically credible counterpoint to the cryptographers opposing the Clipper Chip.

## The PGP Prosecution

[[phil-zimmermann]]'s release of PGP (Pretty Good Privacy) in 1991 — a freely available, strong public-key encryption program — triggered a federal investigation on the theory that making the software available on the internet constituted export to foreign nationals. The Zimmermann case became the defining human story of the Crypto Wars: a programmer faced potential felony prosecution for publishing a mathematical program that any American citizen could use legally for domestic communication.

Schneier supported Zimmermann publicly and consistently. The PGP case illustrated the absurdity of the ITAR regime and its conflict with First Amendment protections for the publication of code and mathematical expressions.

## Daniel Bernstein and the First Amendment

The most legally consequential challenge to ITAR came from [[daniel-bernstein]], a graduate student who challenged the export regulations on First Amendment grounds after being required to obtain a munitions export license to publish his Snuffle encryption algorithm in academic papers. The Bernstein v. U.S. Department of Justice litigation, which the [[electronic-frontier-foundation]] supported, produced a landmark 1999 Ninth Circuit ruling that software source code is protected speech under the First Amendment and that export licensing requirements for cryptographic code were unconstitutional prior restraint.

## Schneier's Applied Cryptography as Political Act

[[applied-cryptography]] (1994) was itself a participant in the Crypto Wars. By publishing a comprehensive reference to cryptographic algorithms with C source code — including export-controlled algorithms — Schneier contributed to making restriction practically unenforceable. The book was exported, referenced, and reproduced. The idea that a textbook's contents could be controlled at national borders was exposed as untenable.

Schneier's position was consistently technical: the argument for export controls rested on the premise that foreign adversaries could not develop or obtain strong cryptography independently. That premise was false; strong cryptography was available from non-U.S. sources. Restricting U.S. cryptographic exports harmed U.S. software companies and U.S. citizens while providing minimal security benefit.

## Resolution and Legacy

The Clinton administration gradually relaxed export controls through the late 1990s under combined pressure from industry, civil liberties organizations, academic researchers, and the courts. By 2000, the export restrictions had been substantially liberalized. The formal end of the Crypto Wars coincided with Schneier's [[security-thinking-pivot]] — his move away from the purely technical framing of the [[cryptography-era]] — but the policy arguments he developed during this period became foundational for all of his subsequent engagement with surveillance, lawful access, and security policy debates.

The Crypto Wars did not end; they evolved. The [[snowden-revelations]] revealed that NSA had pursued the underlying goals of the Crypto Wars through technical subversion rather than legal restriction — compromising encryption standards, inserting backdoors in commercial products, and co-opting the internet infrastructure that the Crypto Wars had ostensibly been fought over.
