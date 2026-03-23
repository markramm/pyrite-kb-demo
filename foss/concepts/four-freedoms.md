---
id: four-freedoms
title: "The Four Freedoms"
type: concept
importance: 8
concept_type: principle
first_appeared: "gnu-manifesto-1983"
key_writings:
- free-software-free-society-2002
- gnu-manifesto-1983
related_concepts:
- copyleft
- open-source-definition
- software-freedom-vs-open-source
tags:
- free-software
- stallman
- fsf
- ethics
- foundational-principle
research_status: draft
---

The four freedoms are the ethical foundation of the free software movement. They are covered in depth in the Stallman KB; this entry focuses on their role as the movement's defining principles and their contrast with the [[open-source-definition]]'s more pragmatic criteria.

[[richard-stallman]] formulated the four freedoms as the conditions that must be met for software to be considered "free" (as in freedom, not price). They are numbered from zero in the hacker tradition: Freedom 0, the freedom to run the program for any purpose; Freedom 1, the freedom to study how the program works and modify it (requiring access to source code); Freedom 2, the freedom to redistribute copies; and Freedom 3, the freedom to distribute copies of your modified versions. These freedoms were articulated gradually through the 1980s and given their canonical numbering and formulation by the [[free-software-foundation]], with the fullest treatment in [[free-software-free-society-2002]]. The [[gnu-manifesto-1983]] contains the philosophical seeds, though the explicit four-freedom formulation came later.

The four freedoms are ethical principles — they define what users deserve, not what makes software development more efficient. This is their fundamental difference from the [[open-source-definition]], which defines "open source" through ten criteria focused on distribution terms: free redistribution, source code availability, derived works, integrity of author's source code, no discrimination against persons or groups, no discrimination against fields of endeavor, distribution of license, license must not be specific to a product, license must not restrict other software, and technology neutrality. The OSD was adapted by [[bruce-perens]] from the Debian Free Software Guidelines for the [[open-source-initiative]] (see [[osi-founding-1998]]). In practice, the two definitions approve nearly identical sets of licenses — almost every license that satisfies the four freedoms also meets the OSD, and vice versa. The difference is in framing and motivation. The four freedoms ask: "Does this license respect the user's autonomy?" The OSD asks: "Does this license meet the criteria for open source distribution?" The answers usually converge, but the questions come from different places, and the divergence in questions produces the divergence in movement politics documented in [[software-freedom-vs-open-source]].

The four freedoms function as an ethical bright line. A piece of software either respects all four freedoms or it does not; there is no gradient. This absolutism is both the principle's strength and its political limitation. Its strength: the four freedoms provide a clear standard that cannot be diluted by corporate marketing or strategic ambiguity. When companies release software under "source-available" licenses like [[sspl-bsl]], the four freedoms provide the test: can users study, modify, and redistribute? If not, the software is not free, regardless of what the marketing says. Its limitation: the absolutism makes the free software position difficult to compromise. [[richard-stallman]]'s refusal to accept "open source" as a legitimate label, his insistence on "GNU/Linux" rather than "Linux," and his objections to permissive licenses that technically satisfy the four freedoms but do not preserve them for downstream users — all reflect the uncompromising quality of the framework.

The four freedoms remain the ethical reference point against which FOSS licensing debates are conducted, even among people who do not identify with the free software movement. When the [[gpl-v3]] added anti-tivoization provisions, the justification was that TiVo's cryptographic lockdown violated Freedom 1 in practice even while respecting it formally. When the [[agpl]] extended copyleft to network use, the justification was that SaaS deployment denied users Freedom 1 and Freedom 3 by never "distributing" the software. The four freedoms are not a historical artifact of the [[gnu-and-free-software-1983-1997]] era; they are the living standard against which new threats to software freedom are measured.
