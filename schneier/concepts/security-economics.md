---
id: security-economics
title: Security Economics
type: concept
tags:
- economics
- incentives
- systems-analysis
- policy
links:
- target: appreciation-for-a-system
  relation: related_to
  note: Schneier's security economics analyzes incentive misalignments in systems, paralleling Deming's appreciation for a system and its sub-optimization dynamics
  kb: deming
- target: enshittification
  relation: related_to
  note: "Both analyze incentive misalignment: Schneier argues security fails when those who can prevent harm don't bear its cost; Doctorow describes the same dynamic in platform value extraction"
  kb: doctorow
- target: institutional-incentives
  relation: related_to
  note: "Parallel claims: Deming argues 94% of quality failures are system-caused; Schneier's security economics argues most security failures are incentive failures"
  kb: deming
- target: management-responsibility-for-quality
  relation: related_to
  note: "Quality as management responsibility maps onto security economics: insecure software exists because vendors don't bear the cost of insecurity"
  kb: deming
- target: evolution
  relation: related_to
  note: Security tools follow Wardley's evolution trajectory (novel → product → commodity); security economics must account for shifting cost structures at each stage
  kb: wardley
- target: inertia
  relation: related_to
  note: "Wardley's inertia maps onto a key security economics failure: organizations treating security as a product when the threat landscape has evolved"
  kb: wardley
- target: institutional-analysis
  relation: related_to
  note: Both analyze how institutional structures systematically misalign incentives
  kb: red-rock-eater
importance: 8
metadata:
  first_appeared: secrets-and-lies
  key_writings: &id001
  - secrets-and-lies
  - beyond-fear
  - schneier-on-security-book
  - data-and-goliath
  - click-here-to-kill-everybody
  related_concepts: &id002
  - security-mindset
  - security-theater
  - security-is-a-process
  - threat-modeling
  - feeling-safe-vs-being-safe
  - trust-framework
  research_status: draft
first_appeared: secrets-and-lies
key_writings: *id001
related_concepts: *id002
research_status: draft
---

Security economics is Schneier's framework for analyzing security failures and security investments through the lens of incentive structures, externalities, and market failures. The central insight — articulated across multiple works beginning with [[secrets-and-lies]] (2000) — is that most security failures are not primarily technical failures but economic ones: the people who could prevent security problems are systematically not the people who bear the cost of those problems.

## The Incentive Misalignment Problem

The foundational argument of security economics is that security markets are systematically distorted because security benefits and security costs are often borne by different parties:

**Software vendors vs. users.** A software company that ships insecure code imposes costs on its users (data breaches, compromised systems) while bearing limited cost itself — because software licenses typically disclaim liability for security failures, because users have limited ability to evaluate software security before purchase, and because switching costs are high once a product is deployed. This is a classic **negative externality**: the vendor captures the revenue while the user bears the security cost.

**Organizations vs. their customers.** An organization that holds customer data bears the reputational and regulatory cost of a breach, but customers bear the direct cost of identity theft, fraud, and exposed personal information. Until data breach notification laws and regulatory fines created accountability, organizations faced systematically weak incentives to invest in data security.

**Individual users vs. their networks.** A computer infected with malware costs the user relatively little (perhaps some performance degradation) while contributing significant cost to everyone else through spam, botnet attacks, and DDoS traffic. This is the **free-rider structure** of internet security: the benefit of maintaining a clean, secure computer is largely external to the individual user.

## The Economic Analysis of Attacks

Security economics also applies to the attacker's side. Schneier argues in [[beyond-fear]] (2003) and subsequent writings that security measures should be evaluated in terms of the costs they impose on attackers relative to the costs they impose on defenders. A security measure that costs $1 million to implement and raises the cost of a successful attack by $100 is a poor investment; one that costs $10,000 and raises attack cost by $1 million is excellent.

This cost-imposition framework explains several counterintuitive security principles:

**Security economics of deterrence.** The value of a security measure often lies not in preventing any single attack but in redirecting adversaries toward softer targets. If your measures make you more costly to attack than your neighbor, attackers may choose the neighbor — even if neither is "secure" against a truly determined adversary.

**The value of uncertainty.** An attacker who doesn't know whether a target has effective defenses must account for the possibility that they do. Unpredictability about security measures can have deterrent value beyond the measures' actual effectiveness.

**The economics of password requirements.** Mandatory password complexity requirements and frequent rotation schedules often reduce security despite their surface plausibility, because they impose significant cognitive costs on users who respond by writing passwords down, reusing them across systems, or choosing patterns that satisfy requirements while remaining guessable. This is a case where the cost imposed on defenders (users) exceeds the cost imposed on attackers, producing negative security economics.

## Ross Anderson's Contribution

Schneier's security economics framework developed in intellectual parallel with [[ross-anderson]]'s work at Cambridge, particularly Anderson's landmark 2001 paper documented in [[anderson-economics-of-information-security]]: "Why Information Security Is Hard: An Economic Perspective." Anderson developed the academic framework for analyzing security as a market failure problem, coining the term "security economics" as a field and documenting the specific market structures (information asymmetry, externalities, monopoly, misaligned liability) that explain why security markets produce systematically poor outcomes.

Schneier and Anderson are intellectual allies on this terrain: both argue that the standard engineering and cryptography communities' focus on technical solutions misses the fundamental driver of security failures, which is economic. Their work is complementary — Anderson's is more formally economic and academic, Schneier's more accessible and policy-oriented.

## Applications to Surveillance

[[data-and-goliath]] (2015) applies security economics to the surveillance economy. Schneier argues that data collection by corporations and governments is a security problem characterized by extreme externalities: the data collected about users imposes risks on those users (data breaches, profiling, manipulation) that are entirely external to the organizations collecting the data. The organizations capture the economic value of the data; the users bear the security risk. Without liability, regulation, or market mechanisms that align these incentives, systematic over-collection and under-protection results.

The [[snowden-revelations]] extended this analysis to government surveillance: the NSA's mass collection programs imposed costs (privacy erosion, chilling effects, infrastructure compromise) on the entire internet ecosystem while the security benefits were concentrated within the intelligence community. Schneier argues this is a textbook case of a security market failure where the costs are diffuse, borne by non-consenting parties, and systematically underweighted.

## Implications for Policy

The security economics framework has direct policy implications:

**Liability.** If software vendors are liable for security failures in their products, they internalize costs that are currently externalized onto users. This aligns incentives toward security investment. Schneier has advocated consistently for software liability reform.

**Mandatory minimum security standards.** Where market forces cannot produce adequate security investment (because consumers cannot evaluate security quality before purchase), regulation can set floors that all vendors must meet. This is the logic of safety regulations in physical products applied to software.

**Data minimization requirements.** If organizations cannot be made liable for the security of data they hold, regulation can reduce the risk surface by limiting how much data they can collect and retain.

In [[click-here-to-kill-everybody]] (2018), Schneier argues that the internet-of-things era makes security economics regulatory questions urgent in a new way: when insecure devices can cause physical harm (through attacks on infrastructure, medical devices, vehicles), the externality structure justifies much stronger regulatory intervention than the computer security failures of the 2000s.
