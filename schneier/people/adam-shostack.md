---
id: adam-shostack
title: "Adam Shostack"
type: person
tags:
- threat-modeling
- security-engineering
- microsoft
- privacy
importance: 7
role: "Security researcher, threat modeling practitioner and author, privacy engineer"
affiliations:
- counterpane-internet-security
research_status: draft
---

Adam Shostack is a security researcher and practitioner who has spent his career at the intersection of security engineering and security practice. He worked with [[counterpane-internet-security]] in the early 2000s and later at Microsoft, where he was the primary developer of the threat modeling practice that became the basis for his definitive book *Threat Modeling: Designing for Security* (2014). He is one of the most systematic practitioners of the [[threat-modeling]] approach that Schneier helped introduce to wider audiences.

## Threat Modeling as Practice

Shostack's central contribution is taking the [[threat-modeling]] concept and turning it into a systematic, teachable engineering discipline. Where Schneier introduced [[attack-trees]] as a formal notation for representing threat structures, and discussed threat modeling as a general approach in [[secrets-and-lies]] and [[beyond-fear]], Shostack developed concrete methodologies — including STRIDE (Spoofing, Tampering, Repudiation, Information disclosure, Denial of service, Elevation of privilege) and the four-question framework — that security teams could apply systematically to real systems.

*Threat Modeling: Designing for Security* (2014) is the most comprehensive practitioner treatment of the subject. It synthesizes Schneier's [[attack-trees]] with Microsoft's security development lifecycle experience and a broader survey of threat modeling approaches, creating a resource that translates the [[security-mindset]] into concrete engineering practice. Shostack has also written about threat modeling for developers who are not security specialists, extending Schneier's project of making security thinking accessible to people who build systems.

## Privacy Engineering

Shostack's work extends to privacy engineering — the systematic application of privacy requirements to system design. This work builds on the same foundations as [[threat-modeling]] but asks about information disclosure and surveillance threats specifically. His collaboration with Andrew Stewart on *The New School of Information Security* (2008) argued for bringing empirical rigor to security claims — testing security assertions against evidence rather than accepting them on authority — which aligns with the [[security-is-a-process]] framework Schneier developed in [[secrets-and-lies]].

The privacy engineering work is particularly relevant to the concerns Schneier developed in [[data-and-goliath]]: if data collection is built into systems from the start, privacy protection must be engineered in from the start, not added later. Shostack has worked to make that engineering tractable and teachable.

## Connection to Counterpane

Shostack's early connection to [[counterpane-internet-security]] placed him in Schneier's professional orbit at a critical period — the early 2000s when Schneier was articulating the [[security-mindset]] and developing the frameworks that would appear in [[beyond-fear]]. The Counterpane community was a gathering point for security practitioners who shared Schneier's orientation: adversarial thinking, systems-level analysis, and skepticism toward security products that promised more than they could deliver.

## Relationship to Schneier

Shostack is primarily an intellectual ally and practitioner who built on Schneier's foundations. The relationship is one of amplification and systematization: Schneier introduced concepts like [[attack-trees]] and [[threat-modeling]] to broad audiences; Shostack developed the methodological discipline that made those concepts operationally useful for security teams. This is a different kind of intellectual relationship than Schneier has with technical cryptography collaborators like [[niels-ferguson]] or [[john-kelsey]] — Shostack's work operates at the level of security practice rather than algorithm design.

Shostack represents the applied wing of Schneier's intellectual influence: practitioners who took Schneier's frameworks and built the methodologies and tools that translate them into daily engineering work. His continued writing and teaching on threat modeling extends the [[security-mindset]] tradition into the next generation of security practitioners.
