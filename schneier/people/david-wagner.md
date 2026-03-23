---
id: david-wagner
title: "David Wagner"
type: person
importance: 5
tags:
- cryptography
- twofish
- security-research
- computer-science
role: "Computer science professor, UC Berkeley"
affiliations: []
relationship_to_schneier: "Twofish co-designer"
research_status: draft
---

David Wagner is a computer science professor at UC Berkeley whose career spans cryptanalysis, applied security, and voting system security. He joined the Twofish team — Schneier, [[niels-ferguson]], [[john-kelsey]], Doug Whiting, and Chris Hall — as a co-designer and cryptanalyst for the [[twofish-algorithm]] submission to the [[aes-competition]], where he contributed primarily to the cipher's security analysis and cryptanalytic resistance arguments.

## Twofish and the AES Competition

The [[aes-competition]] required not just cipher design but rigorous public analysis: the NIST process was designed so that the global cryptographic community could scrutinize all submissions before selection. Wagner's role on the Twofish team included both the design of the cipher's components and the analysis of its security properties — the differential and linear cryptanalysis resistance that teams were required to evaluate for their own submissions. His participation reflected the norms of academic cryptography at the time: serious security claims required people willing to attack their own designs as hard as any external critic would.

The collaboration with Schneier on Twofish occurred during Schneier's most intensive period of technical cryptographic work, the years between [[applied-cryptography]] and the pivot toward security policy that [[secrets-and-lies]] represents. Wagner represents the academic research community — faculty and graduate students at top universities — that the [[aes-competition]] drew into the cipher design process, and whose participation gave the competition much of its credibility.

## Security Research Beyond Cryptography

Wagner's post-AES research extended into application security, including foundational work on SQL injection and other injection attacks, and into electronic voting system security — an area where his technical analysis of specific deployed voting systems showed how [[security-theater]] could masquerade as genuine protection. His voting-systems work parallels Schneier's argument in [[beyond-fear]] that security measures must be evaluated for whether they actually reduce risk, not just whether they appear to do so. Wagner's empirical demonstration that specific voting machines had serious vulnerabilities gave concrete force to the abstract argument that process matters more than product.

His career trajectory illustrates a pattern common to the Twofish-era collaborators: the cipher design work was a moment of concentrated technical collaboration, after which each participant followed their own research direction — but the shared experience of rigorous cryptographic analysis created lasting methodological common ground with Schneier's [[security-mindset]].
