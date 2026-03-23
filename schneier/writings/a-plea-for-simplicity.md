---
id: a-plea-for-simplicity
title: "A Plea for Simplicity: You Can't Secure What You Don't Understand"
type: writing
importance: 6
tags:
- security
- complexity
- essay
- design
- systems
writing_type: essay
date: "1999-11-01"
publisher: "Information Security Magazine"
key_concepts:
- security-is-a-process
- security-mindset
- threat-modeling
research_status: draft
---

"A Plea for Simplicity," published in Information Security Magazine in November 1999, is one of Schneier's strongest statements about the relationship between complexity and security. The central claim is in the subtitle: you cannot secure what you do not understand. Complex systems have complex attack surfaces, and the complexity that makes systems hard to understand for users and administrators makes them equally hard to analyze for defenders — while sophisticated attackers can exploit the complexity asymmetrically.

## The Argument Against Complexity

The essay argues that complexity is the enemy of security for several related reasons:

Security review requires understanding. A cryptographic algorithm can be reviewed and analyzed because it is small and precisely specified. A complex networked system cannot be fully reviewed because no one person understands all of it. Security claims for complex systems therefore rest on incomplete analysis, regardless of the expertise of the reviewers.

Implementation complexity creates attack surface. Every feature, every option, every interface is a potential vulnerability. Systems that minimize features minimize attack surface. Systems optimized for features without security consideration in the design process accumulate vulnerabilities at roughly the rate at which features accumulate.

Operational complexity creates security failures. Complex systems require complex administration. Administrative errors — misconfigurations, incomplete patches, ignored alerts — are among the most common sources of security failures. Simpler systems fail less because there is less to misconfigure.

## The Design Prescription

The essay advocates for security-first design: build the simplest system that meets the requirements, add features only when the security implications have been analyzed, and treat complexity as a cost to be justified rather than a neutral feature to be added freely. This is a design philosophy more than a specific technique, and it sits in tension with the feature-driven product development dominant in the software industry.

The essay connects to Schneier's [[security-mindset]] — the disposition to think about how systems fail, to ask what the minimal attack surface is, to question whether added functionality justifies added risk.

## Context: Late-1990s Software Complexity

The essay was published as internet-connected software was proliferating rapidly and the software industry was engaged in feature wars — competing on the number and novelty of features rather than on reliability, security, or simplicity. The security failures that followed from this period — the epidemic of Internet Explorer vulnerabilities, the compromise of poorly configured UNIX servers, the proliferation of macro viruses — were in significant part consequences of the complexity the essay warned against.

## Position in the Arc

This essay, like [[why-cryptography-is-harder-than-it-looks]], belongs to the late [[cryptography-era]] period when Schneier was developing the arguments that would crystallize in [[secrets-and-lies]]. The complexity argument is one input to the broader claim of Secrets and Lies: that cryptographic correctness is neither necessary nor sufficient for system security, and that system security requires attention to all the human, operational, and design factors that the algorithmic focus of Applied Cryptography had treated as secondary.
