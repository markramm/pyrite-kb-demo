---
id: threat-modeling
title: Threat Modeling
type: concept
tags:
- technical
- methodology
- risk-analysis
- systems-security
links:
- target: ooda-loop
  relation: related_to
  note: Threat modeling structures adversarial observation and orientation; Boyd's OODA loop provides a complementary framework for understanding attacker decision cycles
  kb: boyd
- target: destruction-and-creation-concept
  relation: related_to
  note: Threat modeling requires destroying and rebuilding models as adversaries adapt — Boyd's destruction-and-creation epistemology applied to security
  kb: boyd
- target: situational-awareness
  relation: related_to
  note: Both are structured approaches to understanding a landscape before acting. Wardley maps components and evolution; Schneier models assets, adversaries, and capabilities
  kb: wardley
importance: 8
metadata:
  first_appeared: secrets-and-lies
  key_writings: &id001
  - secrets-and-lies
  - beyond-fear
  - schneier-on-security-book
  - the-process-of-security
  related_concepts: &id002
  - attack-trees
  - security-mindset
  - security-is-a-process
  - security-economics
  - feeling-safe-vs-being-safe
  research_status: draft
first_appeared: secrets-and-lies
key_writings: *id001
related_concepts: *id002
research_status: draft
---

Threat modeling is the structured process of identifying, enumerating, and prioritizing the threats relevant to a specific system, application, or context. In Schneier's work it represents the operationalization of the [[security-mindset]] — the translation of adversarial thinking into an analytical discipline that can be applied systematically rather than relying solely on individual insight.

## Schneier's Contribution

Schneier did not invent threat modeling as a term, but he did more than almost anyone to establish it as a foundational security practice. [[secrets-and-lies]] (2000) argued that security analysis must begin not with technology but with assets and adversaries: what are you protecting, from whom, and what would they do to defeat your protections? This framing — asset-centric and adversary-centric rather than technology-centric — became the intellectual basis for subsequent formal threat modeling methodologies.

The essay [[the-process-of-security]] (2000) makes this most directly: "Security is not a product, it is a process" — and threat modeling is the analytical core of that process. Security requires ongoing assessment of threats, not one-time design.

[[beyond-fear]] (2003) gave the most accessible treatment of threat modeling for general audiences, presenting a five-question framework applicable to any security decision:

1. What assets are you trying to protect?
2. What are the threats to those assets?
3. How well does the security measure mitigate those threats?
4. What other risks does the security measure introduce?
5. What are the costs and trade-offs?

This framework is threat modeling without the technical jargon — usable by policy-makers, business managers, and individuals evaluating everyday security decisions, not just security engineers.

## Relationship to Attack Trees

[[attack-trees]] are a formal technique within the threat modeling process. While threat modeling defines the overall analytical structure — identify assets, identify adversaries, model attack paths, evaluate countermeasures — attack trees provide one specific method for systematically enumerating and analyzing the attack path step. Threat modeling is the process; attack trees are one tool within it. Schneier developed both and they fit together naturally: the threat model identifies what you're defending against, and attack trees formalize how specific adversaries might achieve their objectives.

## The Adversary Model

A crucial element of threat modeling in Schneier's framework is explicit adversary characterization. Who are the realistic attackers? What are their goals, capabilities, constraints, and motivations? This adversary model disciplines the analysis in two directions: it prevents security theater (defending against implausible attackers) and it prevents overconfidence (assuming attackers have only the capabilities that are convenient to imagine).

Schneier regularly distinguishes between:

**Targeted attacks** — adversaries who have specifically chosen a target and will adapt their approach based on the defenses encountered.

**Opportunistic attacks** — adversaries looking for easy targets and moving on if resistance is encountered; effective defenses here raise the cost enough to redirect attackers elsewhere.

The distinction matters enormously for countermeasure selection. A lock that deters an opportunistic attacker is worthless against a targeted one who will simply break the door frame.

## Human Factors in the Threat Model

Schneier's threat modeling consistently incorporates human actors on both sides: human users whose behavior may defeat technical controls, human employees who may be bribed, deceived, or coerced, and human attackers who adapt, innovate, and exploit the gap between designers' assumptions and users' actual behavior. This distinguishes his approach from purely technical security analysis that models attackers as algorithm-executors rather than adaptive agents.

[[liars-and-outliers]] (2012) can be read as an extended meditation on the human dimension of the threat model: the question of which actors in a system will comply with its norms and which will defect, and what social, institutional, and technical mechanisms affect that ratio.

## Influence on Subsequent Practice

Schneier's threat modeling framework influenced the formal methodologies that became standard in software security. [[adam-shostack]]'s STRIDE methodology (developed at Microsoft) and his book *Threat Modeling: Designing for Security* (2014) built directly on the Schneier tradition. STRIDE (Spoofing, Tampering, Repudiation, Information disclosure, Denial of service, Elevation of privilege) is essentially a structured adversary model of the kind Schneier advocated, formalized for the software development context.

The broader discipline of security requirements engineering, which emerged in the early 2000s, also draws heavily on the Schneier framing: that security properties must be specified by analyzing threats, not derived from first principles.

## Threat Modeling Beyond Technology

Like most of Schneier's concepts, threat modeling generalized beyond its technical origins. [[beyond-fear]] applies the five-question framework to physical security, public policy, and everyday personal decisions. [[a-hackers-mind]] (2023) applies it to the analysis of power: who are the actors who might subvert a legal, financial, or political system, what are their objectives, and how do the system's rules create exploitable structure? The threat model becomes a tool for political economy, not just engineering.
