---
id: snowden-revelations
title: "Snowden Revelations"
type: event
importance: 10
tags:
- NSA
- mass-surveillance
- Snowden
- PRISM
- encryption-subversion
- civil-liberties
- internet-trust
date: "2013-06-01"
location: "Hong Kong / global"
participants:
- nsa
- electronic-frontier-foundation
- harvard-kennedy-school
status: confirmed
---

In June 2013, former NSA contractor Edward Snowden disclosed a trove of classified documents to journalists at _The Guardian_ and _The Washington Post_, revealing the scope of NSA and GCHQ mass surveillance programs targeting domestic and international communications. The revelations confirmed and exceeded what security researchers had suspected about government surveillance of internet infrastructure, and they placed Schneier at the center of one of the most significant technology policy events of the decade.

## What the Documents Showed

The Snowden documents revealed multiple surveillance programs operating at scale. PRISM gave NSA access to data held by major U.S. internet companies including Google, Apple, Microsoft, Facebook, and Yahoo, collected under FISA court orders the companies could not disclose. XKeyscore provided analysts with a search engine for intercepted internet communications globally. Upstream programs tapped directly into the fiber optic cables carrying internet backbone traffic.

Most consequentially for the cryptographic community, the documents revealed that [[nsa]]'s Tailored Access Operations (TAO) and related programs had actively worked to subvert encryption standards — including the deliberate insertion of a backdoor into the NIST Dual Elliptic Curve Deterministic Random Bit Generator (Dual EC DRBG), a standard Schneier and others had flagged as suspicious years earlier. The confirmation that NSA had corrupted a NIST standard was a direct reversal of the open evaluation model that the [[aes-competition]] had represented.

## Schneier's Direct Involvement

Schneier worked directly with _The Guardian_ journalist Glenn Greenwald and filmmaker Laura Poitras on the Snowden document coverage, providing technical analysis that helped translate cryptographic and systems concepts into public reporting. He was among the small number of security experts who had the clearance-free technical background to analyze NSA capabilities accurately.

Schneier also wrote extensively on his [[schneier-on-security-blog]] and in major outlets about what the revelations implied. His analysis went beyond the policy dimensions: he explained specifically how the NSA programs worked technically, why the encryption subversion was more dangerous than the data collection, and what the revelations meant for the trustworthiness of internet infrastructure generally. He also pointed readers toward practical countermeasures: [[tor-project]]'s anonymity network, for instance, was one of the tools that the documents showed NSA had found difficult to penetrate, making it a meaningful element of any surveillance-resistance strategy.

## Implications for Trust Infrastructure

For Schneier, the most significant implication of the Snowden revelations was not the existence of surveillance programs — he had expected those — but the systematic subversion of the technical infrastructure of internet trust. NSA had not merely collected data; it had compromised the cryptographic systems that users relied upon for security. This was the [[trust-framework]] analysis of [[liars-and-outliers]] made concrete: the institutions responsible for protecting the security of internet infrastructure had instead weaponized it.

This finding shaped [[data-and-goliath]] (2015), which analyzed the dual surveillance economy — corporate and governmental — as a unified system of power asymmetry. The Snowden context runs through that book and through [[click-here-to-kill-everybody]], which analyzed how internet insecurity extends into physical infrastructure. The revelations accelerated Schneier's transition from [[security-commentator-era]] to [[trust-and-surveillance-era]].

## Policy Consequences

The Snowden revelations prompted significant policy responses: Section 215 of the USA PATRIOT Act was allowed to expire, the USA FREEDOM Act constrained bulk telephony metadata collection, and international tensions over U.S. surveillance affected cloud computing markets and the Safe Harbor privacy framework between the U.S. and EU. None of these changes, in Schneier's analysis, addressed the fundamental structural problem: the alignment of corporate data collection with government surveillance interests that [[data-and-goliath]] documented.

The revelations also strengthened Schneier's relationship with the [[electronic-frontier-foundation]] and reinforced his academic work at [[harvard-kennedy-school]], where the policy dimensions of surveillance and power had become central research questions in the [[trust-and-surveillance-era]].
