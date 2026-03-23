---
id: software-freedom-vs-open-source
title: "Software Freedom vs. Open Source"
type: concept
importance: 8
concept_type: philosophy
first_appeared: "foresight-open-source-meeting-1998"
key_writings:
- cathedral-and-the-bazaar-1997
- gnu-manifesto-1983
- free-software-free-society-2002
- open-sources-anthology-1999
related_concepts:
- commons-based-peer-production
- maintainer-sustainability-crisis
- open-core-business-model
tags:
- philosophy
- free-software
- open-source
- stallman
- raymond
- schism
- foundational-tension
research_status: draft
---

The central philosophical tension of the FOSS movement: two frameworks that share the same licenses, the same code, and largely the same practices, but disagree fundamentally about why any of it matters. Free software, as defined by [[richard-stallman]] and the [[free-software-foundation]], frames software freedom as an ethical imperative — users deserve control over their computing, and software that denies them the [[four-freedoms]] (to run, study, modify, and redistribute) is an injustice regardless of its technical quality. Open source, as articulated by [[eric-raymond]] and institutionalized through the [[open-source-initiative]], frames source availability as a pragmatic methodology — open development produces better, more reliable software, and the business case for openness is stronger than any ethical argument. The term "FOSS" (Free and Open Source Software), and its variant "FLOSS" (Free/Libre and Open Source Software), is itself a diplomatic compromise, acknowledging both camps without endorsing either.

The split became institutional at the [[foresight-open-source-meeting-1998]], when [[christine-peterson]] proposed the term "open source" to replace "free software" in business contexts. The ambiguity of "free" in English — free as in freedom, or free as in beer — had been a persistent obstacle to corporate adoption. "Open source" described the technical characteristic (publicly available source code) without the ideological freight. [[eric-raymond]] and [[bruce-perens]] founded the [[open-source-initiative]] within weeks, and the [[open-source-definition]] (adapted from the Debian Free Software Guidelines) gave the term a formal, certifiable meaning. Stallman refused the new terminology from the start, arguing that stripping the ethical language was not a marketing adjustment but a substantive surrender: if you call it "open source," you invite corporations to adopt the development methodology while ignoring the values that motivated the movement's creation. The schism defined the [[open-source-schism-and-dotcom-1998-2004]] era and has never been resolved.

Stallman's position is that the ethical argument is the load-bearing structure. If FOSS is merely a superior development methodology, then whenever proprietary development proves more efficient for a particular use case, there is no reason to prefer openness. The ethical argument — that proprietary software is wrong because it restricts user freedom — provides a principled floor beneath the pragmatic case. Raymond's counter-position is that the ethical framing alienates exactly the audience the movement needs: corporate decision-makers, enterprise architects, government procurement officers. By speaking in terms of engineering quality, security through transparency, and reduced vendor lock-in, the open source movement achieved adoption that the free software movement never could. The corporate embrace of Linux, Apache, and eventually the entire cloud computing stack during the [[mainstream-adoption-and-corporate-embrace-2005-2014]] era is, in this view, vindication of the pragmatic strategy.

The tension plays out concretely in licensing and business models. The [[free-software-foundation]] stewards the [[gpl-v2]] and [[gpl-v3]], copyleft licenses designed to ensure that freedom propagates — if you use GPL code, your derivative work must also be GPL. The open source ecosystem increasingly favored permissive licenses ([[mit-license]], [[apache-license-2]], [[bsd-license]]) that allow proprietary incorporation, reflecting the pragmatic view that maximum adoption matters more than enforcing downstream freedom. The rise of the [[open-core-business-model]] sits squarely in this tension: companies release a core under a permissive or copyleft license, then add proprietary extensions — a practice the OSI tolerates and the FSF views as a compromise of user freedom. The [[sspl-bsl]] licenses of the late 2010s introduced a new wrinkle: licenses that look open but restrict commercial use, rejected by both the OSI (not open source) and the FSF (not free software), satisfying neither camp.

The question of whether this philosophical tension matters practically or only academically was answered by the [[maintainer-sustainability-crisis]] and the [[modern-foss-and-sustainability-crisis-2015-present]] era. When corporations extract billions in value from FOSS while maintainers work unpaid, the ethical framing (corporations owe the community) and the pragmatic framing (the ecosystem needs better funding mechanisms) converge on the same diagnosis but diverge on remedies. The [[linux-foundation]]'s OpenSSF model (corporate co-investment in shared infrastructure) reflects the open source pragmatist approach. The [[software-freedom-conservancy]]'s GPL enforcement and advocacy reflects the free software ethical approach. Whether the movement is one movement with two vocabularies or two movements sharing a codebase remains, more than twenty-five years after the Foresight meeting, genuinely unresolved.
