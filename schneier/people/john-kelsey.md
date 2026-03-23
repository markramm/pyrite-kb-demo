---
id: john-kelsey
title: "John Kelsey"
type: person
tags:
- cryptography
- co-author
- twofish
- nist
importance: 7
role: "Cryptographer at NIST, frequent Schneier co-author on technical papers and algorithm design"
affiliations:
- nist
- counterpane-internet-security
research_status: draft
---

John Kelsey is a cryptographer who worked with Bruce Schneier on some of his most technically significant output and has been a long-term collaborator at [[nist]], where he contributes to cryptographic standards development. Of all Schneier's technical collaborators, Kelsey produced the most co-authored papers — the working relationship spanned from the [[counterpane-internet-security]] period through years of joint cryptanalytic work.

## Technical Contributions

Kelsey's research spans symmetric cryptography, hash functions, random number generation, and protocol design. He contributed to important cryptanalytic results — including work on related-key attacks, slide attacks, and the analysis of hash function constructions — that shaped how the field understood the security of deployed systems. At [[nist]], he has been deeply involved in the SHA-3 hash function competition and subsequent standards work, continuing the pattern of bridge-building between research cryptography and deployable standards.

His independent contributions include work on cryptographic random number generation (with implications for the famous Dual EC DRBG backdoor controversy that emerged after the [[snowden-revelations]]) and on the security properties of various chaining modes for block ciphers. This work is technical in a way that does not translate easily into the policy discussions Schneier increasingly engaged, but it provides the empirical foundation that makes policy arguments credible.

## Twofish Collaboration

Kelsey was a core member of the [[twofish-algorithm]] design team alongside Schneier, [[niels-ferguson]], Doug Whiting, David Wagner, and Chris Hall. The [[aes-competition]] required not just a cipher submission but extensive supporting analysis, and Kelsey contributed to the security arguments and cryptanalytic testing that accompanied the Twofish submission. The collaboration with Kelsey during this period gave Schneier direct access to someone who could stress-test cipher designs from an attacker's perspective — the same adversarial stance that would later become the [[security-mindset]] concept.

## Paper Co-Authorship

Beyond Twofish, Kelsey and Schneier co-authored numerous technical papers in the mid-to-late 1990s and early 2000s. These included papers on related-key attacks (showing that some ciphers thought to be secure had exploitable weaknesses when keys were related), randomness and pseudorandomness, and the security of specific constructions. The volume of this collaboration means that Kelsey was present for much of the period when Schneier was developing the [[attack-trees]] formalism and thinking through the conceptual frameworks that would appear in [[secrets-and-lies]] and [[beyond-fear]].

## Role in Schneier's Technical Network

Kelsey represents a category of Schneier collaborator distinct from [[niels-ferguson]] or [[ross-anderson]]: a working cryptographer whose interaction with Schneier was primarily through joint research papers rather than through co-authorship of books or public policy debates. These technical collaborations matter for understanding Schneier's intellectual development because they document his engagement with the research frontier at a level of detail that his popular books do not. The papers Kelsey and Schneier produced together show a Schneier thinking carefully about adversarial attack scenarios — the same habits of mind that would eventually broaden into the generalized [[security-mindset]] and [[hacking-as-systems-subversion]] frameworks. Kelsey's continued work at [[nist]] also keeps him at the intersection of cryptographic research and standards — exactly the institutional context that Schneier has analyzed and advocated around for decades.
