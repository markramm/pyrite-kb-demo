---
id: daniel-bernstein
title: "Daniel J. Bernstein"
type: person
tags:
- cryptography
- crypto-wars
- first-amendment
- legal-case
- djb
importance: 7
role: "Mathematician and cryptographer, plaintiff in Bernstein v. DOJ, designer of influential cryptographic software"
affiliations:
- electronic-frontier-foundation
research_status: draft
---

Daniel J. Bernstein (known as djb, b. 1971) is a mathematician and cryptographer at the University of Illinois at Chicago and Eindhoven University of Technology. He is known for two distinct contributions: the landmark First Amendment lawsuit *Bernstein v. United States Department of Justice*, which became the lead constitutional challenge to cryptography export controls, and a body of cryptographic software — including Curve25519, ChaCha20, and Poly1305 — that has become foundational infrastructure for modern secure communications.

## Bernstein v. DOJ

In 1995, Bernstein — then a graduate student at UC Berkeley — filed suit against the US government after being informed that his Snuffle encryption software and the academic paper describing it could not be posted online without an export license. He argued that software source code was protected speech under the First Amendment and that the export control regime was an unconstitutional prior restraint.

The case, backed by the [[electronic-frontier-foundation]], proceeded through the courts for years and produced a significant 1999 Ninth Circuit ruling holding that software source code was expressive speech protected by the First Amendment — a major legal blow to the [[crypto-wars-export-controls]]. The ruling was eventually vacated on procedural grounds when the Clinton administration relaxed export controls, but it established important precedent and demonstrated that the constitutional arguments against crypto restrictions had merit.

Bernstein's case ran in parallel with the government's criminal investigation of [[phil-zimmermann]], but where Zimmermann was a defendant who had not sought confrontation, Bernstein was a plaintiff who deliberately picked the fight. His suit exemplified the strategy of using the legal system as an arena for the crypto policy debate — a strategy the [[electronic-frontier-foundation]] pursued across multiple fronts during the [[crypto-wars-export-controls]] period.

## Cryptographic Contributions

Bernstein's technical contributions became significant well after the legal battle. He designed a series of cryptographic primitives that achieved wide adoption because of their combination of strong security arguments, clean implementation, and resistance to the timing side-channel attacks that plagued older designs. Curve25519 (an elliptic curve for key agreement), ChaCha20 (a stream cipher), and Poly1305 (a message authentication code) — packaged together as NaCl (Networking and Cryptography Library) — are now used in TLS, SSH, Signal, and many other deployed systems.

Bernstein's design philosophy is to make it easy to use cryptography correctly and hard to use it incorrectly — exactly the practitioner orientation that [[practical-cryptography]] advocates. His insistence on conservative security margins and his willingness to publicly challenge NIST algorithm choices (including his ongoing criticism of potential NSA influence on elliptic curve standards, concerns later amplified by the [[snowden-revelations]]) reflect the same adversarial skepticism that characterizes Schneier's [[security-mindset]].

## Relationship to Schneier

Bernstein and Schneier engaged the same [[crypto-wars-export-controls]] debates from different angles: Schneier through public writing, consulting, and policy advocacy; Bernstein through a constitutional lawsuit and technical research. Their relationship is that of fellow travelers who never closely collaborated but shared the same adversary and the same basic position: that the government's attempt to control civilian access to cryptography was both technically misguided and constitutionally indefensible.

Schneier's [[crypto-gram-newsletter]] and broader writing during the 1990s and early 2000s regularly documented and praised the work being done to challenge export controls — work that Bernstein's lawsuit exemplified. The eventual liberalization of export controls in the late 1990s was a collective victory for this network of legal, technical, and policy opposition in which both Bernstein and Schneier played significant roles.
