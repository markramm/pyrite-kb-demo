---
id: free-software-definition
title: The Free Software Definition
type: concept
tags:
- free-software
- definition
- philosophy
- legal
importance: 9
concept_type: philosophical
first_appeared: free-software-definition-essay (1996, gnu.org)
key_writings:
- free-software-definition-essay
- gnu-manifesto
- why-software-should-be-free
- free-software-free-society
related_concepts:
- four-freedoms
- copyleft
- libre-vs-gratis
- free-as-in-freedom-concept
- software-freedom-vs-open-source
research_status: draft
---

The Free Software Definition is [[stallman]]'s formal specification of what makes software "free" in the sense he intends. Published on gnu.org (first canonically in 1996, though the underlying ideas are older), it states that a program is free software if it provides all [[four-freedoms]] to every user: the freedom to run, to study, to redistribute, and to modify and redistribute modified versions.

The definition exists to settle a precise question: not whether software is free of charge, but whether it respects the user's freedom. The [[libre-vs-gratis]] and [[free-as-in-freedom-concept]] distinctions exist precisely because English conflates these two meanings of "free."

## Structure of the Definition

The Free Software Definition is binary: software either satisfies all four freedoms or it does not. Partial satisfaction — software that permits three of the four — is still non-free software by Stallman's definition. This all-or-nothing structure reflects his philosophical position that freedom is not divisible: a single restriction is enough to subject users to the developer's power.

The definition specifies freedoms, not features. It says nothing about price, quality, documentation, or developer community. Software can be expensive and still be free software (in the relevant sense); software can be gratis and still be non-free if it withholds source code or restricts modification.

## What the Definition Excludes

The definition is explicit about what does not make software non-free: requiring attribution, requiring that modifications be released (copyleft), requiring that the original author's name not be used to endorse derivatives, or requiring that derived works use a different name. These are conditions on distribution, not restrictions on freedom.

What does make software non-free: restricting the right to run (use-case restrictions), withholding source code, prohibiting redistribution, or prohibiting modification. Any one of these disqualifies a program.

## Relationship to Open Source

When [[eric-raymond]] and [[bruce-perens]] founded the [[open-source-initiative]] in 1998, they produced the Open Source Definition — a parallel document with ten criteria for open source licenses. The OSI definition is substantially similar to the Free Software Definition but admits some licenses that [[stallman]] considers non-free (particularly licenses with field-of-use restrictions or discriminatory clauses). [[stallman]]'s position is that the two definitions mostly agree in practice but differ in philosophy and occasionally in specifics — see [[software-freedom-vs-open-source]].

## Living Document

The Free Software Definition on gnu.org has been updated over the years to address new edge cases — tivoization, SaaS, DRM. When the [[gpl-v3]] was drafted, the definition was revised to clarify that Freedoms 1 and 3 require that modification and installation be practically possible, not just legally permitted. This is the philosophical underpinning of the anti-[[tivoization]] clause in GPLv3.

## Authority

The Free Software Definition is maintained by the [[free-software-foundation]] and is the authoritative statement of what counts as free software for FSF purposes. The FSF licenses list and the GNU package acceptance criteria both use it as the test. It is the foundation on which [[stallman]]'s entire project rests: every argument he makes about proprietary software, every campaign against DRM or software patents, presupposes this definition of what freedom means in the software context.
