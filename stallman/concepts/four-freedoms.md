---
id: four-freedoms
title: The Four Freedoms
type: concept
tags:
- free-software
- philosophy
- definition
- foundational
links:
- target: egoless-programming
  relation: related_to
  note: Stallman's four freedoms treat code as a shared commons; Weinberg's egoless
    programming treats code as belonging to the team rather than the individual —
    both oppose proprietary ownership of software
  kb: weinberg
- target: selective-amplification
  relation: related_to
  note: 'Agre''s selective amplification argues that technology design is inherently
    political because it chooses which social forces to strengthen. Stallman''s four
    freedoms are a normative answer to the same question: software design should amplify
    user autonomy rather than vendor control.'
  kb: red-rock-eater
- target: security-mindset
  relation: related_to
  note: Freedom 1 (the right to study how a program works) is a prerequisite for Schneier's
    security mindset — you cannot evaluate whether software is secure if you cannot
    read its source. Schneier's DRM security critique is essentially the security-mindset
    argument for Freedom 1.
  kb: schneier
- target: evolution
  relation: related_to
  note: Wardley's evolution framework predicts that components move toward commodity
    and that openness accelerates this. Stallman's four freedoms provide the normative
    framework for what openness means. Wardley sees openness as an evolutionary force;
    Stallman insists it is an ethical requirement.
  kb: wardley
importance: 10
concept_type: philosophical
first_appeared: gnu-manifesto (1985), formalized in free-software-definition-essay
  (1996)
key_writings:
- gnu-manifesto
- free-software-definition-essay
- why-software-should-be-free
- free-software-free-society
related_concepts:
- free-software-definition
- copyleft
- free-as-in-freedom-concept
- libre-vs-gratis
- software-freedom-vs-open-source
research_status: draft
---

The four freedoms are the core normative framework of [[stallman]]'s free software philosophy — a precise, numbered definition of what it means for software to be free. They are:

- **Freedom 0**: The freedom to run the program as you wish, for any purpose.
- **Freedom 1**: The freedom to study how the program works, and change it so it does your computing as you wish. Access to the source code is a precondition for this.
- **Freedom 2**: The freedom to redistribute copies so you can help others.
- **Freedom 3**: The freedom to distribute copies of your modified versions to others. Access to the source code is a precondition for this.

The numbering starting at zero is deliberate — [[stallman]] was a programmer, and in many languages arrays are zero-indexed. Freedom 0 (to run) was added later as an explicit clarification; early formulations implied it but did not state it.

## Origin and Development

The intellectual germ appears in the [[gnu-manifesto]] (1985), whose [[gnu-manifesto-concept|philosophical argument]] centers on software users' right to share and modify programs. But the four freedoms as a numbered list were not formally codified until the mid-1990s, when the [[free-software-foundation]] needed a precise definition to distinguish free software from freeware, shareware, and semi-open licenses. The [[free-software-definition-essay]] (1996 on gnu.org) is the canonical published formulation.

Stallman had been using the underlying concepts since the early 1980s — the requirement for source code access, the right to share, the right to modify — but the four-part structure gave the philosophy a teachable, enforceable shape.

## Why Four, and Why These Four

The four freedoms are not a random enumeration; they address every point at which a software vendor might restrict a user. Proprietary software restricts running (through licenses that limit use cases), studying (through withholding source code), redistributing (through copyright and contract), and modifying (through the same). Each freedom addresses a specific mode of control.

[[stallman]] consistently emphasizes that all four are necessary; removing any one produces software that is not free in the relevant sense. A program that provides Freedoms 1-3 but restricts Freedom 0 — for example, software you can modify but only run for non-commercial purposes — is not free software by this definition.

## The Precondition of Source Code

Freedoms 1 and 3 explicitly require access to source code. This is not incidental — it is a direct response to the practice of distributing software only in compiled binary form, which makes it effectively opaque to study and difficult to modify. The [[gpl-copyleft-mechanism]] enforces this by requiring that any distributed binary include or be accompanied by the corresponding source code.

## Relationship to the Free Software Definition

The four freedoms are the substance of the [[free-software-definition]]. The definition says software is free if and only if it provides all four freedoms to all users. This makes the definition binary rather than scalar — software is either free or it is not, regardless of how many restrictions it places or how reasonable those restrictions might seem.

This all-or-nothing structure was deliberate and has been a persistent point of contention. Critics argue it is too rigid; [[stallman]] argues that any exception creates a hole through which non-freedom can enter.

## Influence

The four freedoms framework was adopted and adapted by the [[open-source-initiative]] in its [[open-source-definition-schism]], though the OSI's "open source definition" uses different language and allows some restrictions that the four freedoms forbid. [[stallman]] regards this as a fundamental philosophical error — see [[software-freedom-vs-open-source]].

The framework influenced [[larry-lessig]]'s [[creative-commons]] project, which applied similar thinking to creative works more broadly. The [[free-as-in-freedom-concept]] distinction — free as in freedom, not free as in beer — is the popular shorthand for what Freedom 0 through Freedom 3 try to specify precisely.

The four freedoms are the benchmark against which [[stallman]] evaluates every license, policy, and software project. Anything that fails on any of the four is, from his perspective, a tool of user subjugation rather than user empowerment.
