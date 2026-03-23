---
id: schneiers-law
title: Schneier's Law
type: concept
tags:
- cryptography
- epistemology
- security-evaluation
- professional-norms
links:
- target: copyleft
  relation: related_to
  note: Schneier's law (don't roll your own crypto) and Stallman's copyleft both argue
    that distributed, expert-reviewed commons outperform proprietary closed solutions
  kb: stallman
importance: 7
first_appeared: '1998'
key_writings:
- secrets-and-lies
- applied-cryptography
- why-cryptography-is-harder-than-it-looks
- a-plea-for-simplicity
related_concepts:
- security-mindset
- security-is-a-process
- attack-trees
- threat-modeling
- security-economics
research_status: draft
---

Schneier's Law is the informal name for the aphorism: "Anyone can invent a security system so clever that he or she can't think of a way to break it." The term was coined by Cory Doctorow, who named the principle after Schneier in the mid-2000s. The law articulates a fundamental epistemological problem in security design: absence of known vulnerabilities is not evidence of security, because the designer's inability to break their own system proves only the limits of the designer's imagination, not the system's actual strength.

## The Underlying Argument

The law captures an asymmetry between construction and analysis in security systems. Building a system that appears secure to its designer is far easier than building a system that is actually secure, because:

**Designers know their intended use case.** They have optimized for the scenario they imagined and have naturally blind spots about scenarios they did not. An attacker, unburdened by the designer's assumptions, can approach the system with fresh eyes and notice gaps the designer didn't consider.

**Security properties are difficult to prove.** Most engineering disciplines allow quality verification through testing — a bridge either holds the weight or it doesn't; a drug either produces the clinical outcome or it doesn't. Cryptographic and security systems cannot be verified this way. A system can pass all tests that the designer thinks to run and still be catastrophically broken against a test the designer didn't think of.

**The smart-person fallacy.** The more clever and technically sophisticated the designer, the more confident they may be that no one can break their system. But sophistication in design does not guarantee that the design is actually correct; it may instead mean the designer has constructed a more elaborate version of a fundamentally flawed approach.

## Historical Context

The law reflects hard-won experience from the cryptography community. The history of cryptography through the mid-20th century is populated with systems that their designers believed secure and that expert analysts later broke — often with elegant, simple attacks that the designers would have considered if they had asked the right questions. The development of modern cryptography as a discipline was partly driven by the recognition that informal security reasoning was systematically overconfident.

Schneier articulated this concern explicitly in [[why-cryptography-is-harder-than-it-looks]] (1997), one of his most important essays, which argued that the difficulty of evaluating cryptographic security meant that amateur cryptography was almost always broken, that only extensive expert analysis could build justified confidence in a system's security, and that the appropriate default response to an unvetted security system was skepticism regardless of how clever it appeared.

[[applied-cryptography]] (1994) provided much of the technical substrate for these arguments — its descriptions of cryptanalytic techniques are partly a demonstration of how sophisticated the "breaking" side of the problem is, which makes clear why the designer's inability to break a system proves little.

## Application to Real-World Failures

The law explains a recurrent pattern in security failures: roll-your-own cryptography. Despite explicit advice from Schneier and the broader security community that custom cryptographic implementations are almost always insecure, organizations repeatedly build proprietary encryption schemes that the developers are confident are secure. These schemes are then broken, sometimes by elementary attacks.

The pattern is not limited to cryptography. Custom authentication systems, home-brew access control mechanisms, and proprietary security protocols that developers built because they "didn't understand what the standard options were doing" are all instances of the same phenomenon: the designer couldn't think of a way to break it, and this didn't mean it was secure.

[[a-plea-for-simplicity]] (1999) addresses the related failure mode of overbuilt complexity: systems with too many features and options are harder to analyze for security precisely because the attack surface is larger. The simpler a system, the more thoroughly it can be analyzed; complexity increases the probability that something is broken somewhere that neither the designer nor any reviewer has found.

## Relationship to Peer Review and Open Design

The positive implication of the law — what it implies designers and organizations should do — is that security systems require external, adversarial review by people who are trying to break them. This is the Kerckhoffs's principle side of the argument: security should derive from the strength of keys and algorithms, not the secrecy of design, because secret designs prevent the external review that builds justified confidence.

Schneier has been a consistent advocate for public cryptographic standards evaluated through open competition processes, as exemplified by the [[aes-competition]] (1997-2001), in which [[twofish-algorithm]] — his team's submission — was one of five finalists. The open competition model directly embodies the epistemological lesson of the law: the only way to build justified confidence in a security system is to expose it to the best analysts who can be found trying to break it.

## The Law and Professional Humility

Schneier's Law applies to Schneier himself. His public acknowledgment of [[applied-cryptography]]'s limits in [[secrets-and-lies]] can be read as an act of intellectual honesty consistent with the law: he had designed the conceptual framework of that book, he had believed in it, and he had come to recognize that he had missed something important about how security actually fails. The law is not just a warning about others' overconfidence; it is an explicit commitment to epistemic humility about one's own.

[[niels-ferguson]] and [[john-kelsey]], Schneier's collaborators on [[twofish-algorithm]] and [[practical-cryptography]], represent the collaborative adversarial review model in practice: systems built by experts working in teams, explicitly trying to identify each other's errors, produce better security than systems built by any individual designer no matter how clever.
