---
id: ietf
title: "Internet Engineering Task Force"
type: organization
importance: 6
tags:
- internet-standards
- cryptography
- protocols
- open-standards
org_type: standards-body
founded: "1986"
location: "Distributed (no fixed location)"
url: "https://www.ietf.org"
---

The Internet Engineering Task Force (IETF) is the primary standards body for internet protocols and technical infrastructure. It develops and maintains the standards that govern how internet communications work — including the cryptographic protocols that secure those communications. Schneier's relationship with the IETF spans his [[cryptography-era]] involvement with protocol security analysis through his ongoing advocacy for open, transparent standards processes.

## Role in Internet Security Standards

The IETF operates through an open, consensus-based process: anyone can participate in working groups, all discussions are public, and standards documents (RFCs — Requests for Comments) are freely available. This model is consistent with Schneier's principle that security requires open analysis rather than trusted authority, and IETF's cryptographic work has been a recurring reference point in his writing.

Key internet security protocols developed or standardized through the IETF process include TLS (Transport Layer Security), IPsec (Internet Protocol Security), SSH (Secure Shell), and DNSSEC (DNS Security Extensions). Schneier has analyzed these protocols in [[applied-cryptography]] and subsequent writing, using them as examples of both good security design (where the open IETF process has worked well) and security failures (where implementation complexity, vendor influence, or political compromise has introduced weaknesses).

## Counterpane and IETF Engagement

[[counterpane-internet-security]] engaged with IETF standards work, consistent with Schneier's practice of contributing to the public security infrastructure. Researchers affiliated with Counterpane participated in working groups relevant to their areas of expertise. This engagement reflected a consistent theme in Schneier's work: security improvements must be implemented at the protocol and infrastructure level, not only in individual applications, and contributing to standards bodies is one mechanism for achieving that.

## NSA Influence on IETF Standards

The [[snowden-revelations]] revealed that [[nsa]] had influenced IETF standards in ways that weakened security for surveillance purposes. The most significant documented instance was the Dual EC DRBG case, which involved [[nist]] standardization rather than IETF directly, but Snowden documents also revealed efforts to compromise TLS and other IETF-standardized protocols through implementation vulnerabilities and key compromise.

For Schneier, this represented the same structural problem as the [[nist]] cases: the open standards process, which he valued and participated in, was vulnerable to subversion by powerful actors with the resources and institutional access to shape it from within. The IETF's openness makes it somewhat more resistant than closed processes to covert corruption — the discussions are public, which increases the cost of manipulation — but as the Snowden materials showed, the resistance was not complete.

## Standards as Security Infrastructure

Schneier's engagement with IETF reflects his broader view that internet security is fundamentally a public infrastructure problem. The protocols that secure internet communications are shared infrastructure: their security properties affect everyone who uses them, not just the parties to any individual communication. This makes standards bodies like IETF important governance institutions, not merely technical conveniences.

This analysis connects to the [[trust-framework]] argument of [[liars-and-outliers]] and the systems-subversion analysis of [[a-hackers-mind]]: shared infrastructure creates shared dependencies, and those dependencies are potential points of leverage for powerful actors who can shape the infrastructure to serve their interests rather than everyone's.
