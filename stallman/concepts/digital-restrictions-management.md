---
id: digital-restrictions-management
title: Digital Restrictions Management (DRM)
type: concept
tags:
- drm
- digital-restrictions
- rhetoric
- technical
- advocacy
links:
- target: digital-rights-management-critique
  relation: related_to
  note: Stallman's DRM opposition directly parallels Doctorow's sustained critique
    of DRM as a tool of corporate control over user devices
  kb: doctorow
- target: capture-model
  relation: related_to
  note: 'DRM systems are a concrete implementation of Agre''s capture model: they
    impose grammars of action on media consumption by requiring authentication, tracking
    usage, and restructuring informal activity into discrete, server-mediated, recordable
    events.'
  kb: red-rock-eater
- target: security-theater
  relation: related_to
  note: DRM does not prevent determined copying but restricts legitimate users, making
    it analogous to security theater — visible measures that provide the appearance
    of protection without meaningful effectiveness, while imposing real costs on users
    and real security vulnerabilities through code opacity.
  kb: schneier
importance: 8
concept_type: rhetorical
first_appeared: Stallman began using 'Digital Restrictions Management' in public writing
  circa 2000-2001
key_writings:
- can-you-trust-your-computer
- free-software-free-society
- gpl-v3
related_concepts:
- four-freedoms
- tivoization
- right-to-read
- software-patents-opposition
- gpl-copyleft-mechanism
research_status: draft
---

"Digital Restrictions Management" is [[stallman]]'s reframing of the industry term "Digital Rights Management" (DRM). The rename is deliberate and substantive: where the industry term positions DRM as protecting rights (of content owners), Stallman's version describes what DRM actually does — restrict what users can do with content and software they have legitimately obtained.

## The Rhetorical Argument

The term "Digital Rights Management" frames the technology from the perspective of content producers: they have rights (copyright), and DRM manages those rights. [[stallman]]'s counterargument is that the rights the industry is "managing" are the user's rights — specifically, the right to use content in ways that copyright law permits (fair use, format shifting, private copying) but DRM systems prevent.

By renaming DRM "Digital Restrictions Management," Stallman shifts the frame: the question is not whether content owners have rights (they do) but whether the technical mechanisms used to enforce those rights are proportionate and whether they restrict users beyond what copyright law actually requires.

## Technical Mechanisms

DRM systems typically involve:

1. **Encryption**: Content is encrypted; decryption is controlled by the DRM system.
2. **Authentication**: Players or devices must authenticate with a server to obtain decryption keys.
3. **Hardware enforcement**: Players are designed to refuse to output unencrypted content ([[tivoization]] is the hardware version of this for software).
4. **Legal backing**: The US Digital Millennium Copyright Act (DMCA) and the EU Copyright Directive make circumventing DRM illegal, even for lawful purposes — a restriction that goes beyond copyright itself.

The DMCA provision prohibiting circumvention is central to [[stallman]]'s critique: it converts a technical mechanism into a legal one, making it illegal to exercise rights that copyright law does not actually prohibit. A user who wants to exercise their fair use rights cannot legally circumvent DRM to do so, even if the underlying copyright use would be lawful.

## The Right to Read Connection

[[stallman]]'s essay [[right-to-read-essay]] (1997) anticipated the DRM era with a dystopian story about a future where all reading is monitored and controlled through technical systems. The essay was prescient: DRM systems do in fact track what users read (e-books), watch (streaming services), and play (video games), reporting usage back to servers.

The [[right-to-read]] concept connects DRM to a broader surveillance concern: DRM is not just restriction but monitoring. When content can only be accessed through authenticated, server-connected systems, those systems necessarily know what you are accessing and when.

## GPLv3 and Anti-DRM Provisions

[[gpl-v3]] (2007) addressed DRM in two ways:

1. **Anti-tivoization (Section 6)**: Required that user products receiving GPL software come with the means to install modified versions — preventing hardware DRM from defeating software freedom (see [[tivoization]]).

2. **DRM circumvention (Section 3)**: Stated that GPL-licensed software does not count as a "technological protection measure" under the DMCA or similar laws, meaning that circumventing GPL software cannot be treated as a DMCA violation. This prevents GPL-licensed code from being used as a DRM layer that would restrict users.

## Defective by Design

The [[free-software-foundation]] runs the "Defective by Design" campaign specifically targeting DRM products — labeling them defective because the restriction is a design choice, not an accident. The campaign names and publicizes specific DRM systems and products. [[stallman]] considers DRM fundamentally incompatible with user freedom and will not use DRM-restricted products. He has extended this critique to surveillance integrated into ostensibly free software, as in his analysis of [[ubuntu-spyware]], where Ubuntu's integration with Amazon's servers represents a DRM-adjacent restriction on what users can control.

## Broader Context

[[stallman]] situates DRM within a pattern of threats to user freedom that also includes [[software-patents-opposition]] and proprietary software licensing. All three use legal or technical mechanisms to prevent users from controlling their own computing. DRM is distinctive in applying these restrictions to content rather than software — but the [[four-freedoms]] framework implies analogous rights for users of content: the right to read, copy, and share within the bounds of copyright law.
