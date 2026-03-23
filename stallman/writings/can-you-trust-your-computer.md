---
id: can-you-trust-your-computer
title: "Can You Trust Your Computer?"
type: writing
importance: 8
tags:
- trusted-computing
- drm
- free-software
- surveillance
- palladium
- essay
writing_type: essay
date: 2002-10-01
coauthors: []
publication: "GNU Project / Free Software Foundation"
url: "https://www.gnu.org/philosophy/can-you-trust.html"
key_concepts:
- digital-restrictions-management
- tivoization
- four-freedoms
- free-software-definition
- right-to-read
research_status: draft
---

"Can You Trust Your Computer?" (2002) is [[stallman]]'s analysis of "trusted computing" — specifically Microsoft's "Palladium" initiative (later renamed "Next-Generation Secure Computing Base") and the Trusted Computing Platform Alliance (TCPA). The essay's central rhetorical move, which became widely influential, is reversing the question embedded in the phrase "trusted computing": trusted by whom? A system designed so that content owners and software vendors can trust that the hardware will enforce their restrictions is a system that users cannot trust to act in their interests.

The essay identifies the threat concisely. Trusted computing hardware (TPM chips) and the software infrastructure built on them would enable: (1) remote attestation — the ability of a remote server to verify what software is running on a user's machine; (2) sealed storage — encryption of data in ways tied to specific software, so that software updates or replacements would lose access to the user's own data; (3) curtained memory — software hidden from the user's inspection even while running on their hardware.

[[stallman]]'s analysis is that these capabilities, while technically described as security features, are primarily mechanisms of control. Remote attestation would allow content distributors to refuse service to computers running software they haven't approved — meaning GNU/Linux systems could be locked out of services, documents, and media. Sealed storage would make it impossible to migrate data when switching software. Curtained memory would make it impossible to inspect what programs are actually doing.

The connection to [[digital-restrictions-management]] is direct: trusted computing is the hardware layer that makes [[digital-restrictions-management|DRM]] enforceable in ways that pure software cannot achieve, because software DRM can always be reverse-engineered on hardware the user controls. With trusted computing hardware, the user's own computer becomes an adversary.

This essay was widely read and influenced thinking at [[electronic-frontier-foundation]] and elsewhere. It connects directly to the later development of [[gpl-v3]]'s anti-[[tivoization]] clause: [[tivoization]] is precisely the scenario "Can You Trust Your Computer?" describes — using hardware to prevent users from running modified software. The essay also connects to [[right-to-read-essay]]: the dystopian future [[stallman]] sketched in 1997 now had specific technical mechanisms named and described.

The essay was written during the [[free-vs-open-source-schism-1998-2007]] era, when debates about software freedom were moving from licensing to hardware and infrastructure. [[eric-raymond]] and the open source camp generally downplayed these concerns as ideological; the [[free-software-foundation]] position was that they were the natural consequence of not insisting on user freedom from the beginning.
