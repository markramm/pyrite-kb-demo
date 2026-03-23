---
id: platform-decay-cycle
title: "Platform Decay Cycle"
type: concept
tags:
- platform-economics
- monopoly
- digital-rights
- antitrust
links:
- target: grammars-of-action
  relation: related_to
  note: Agre's grammars of action — formal representations that decompose activities into trackable steps — describe the mechanism by which platforms impose lock-in behavioral loops
  kb: red-rock-eater
- target: institutional-coevolution
  relation: related_to
  note: Agre's institutional coevolution — technology and institutions mutually reshaping each other — is the macro framework behind platform decay
  kb: red-rock-eater
importance: 8
metadata:
  first_appeared: "Synthesized across Doctorow's blog writing and talks, 2019–2023; crystallized in enshittification formulation (2023)"
  key_writings: &id001
  - pluralistic-blog
  - the-internet-con
  - enshittification-talk-defcon
  - chokepoint-capitalism-book
  related_concepts: &id002
  - enshittification
  - switching-costs
  - adversarial-interoperability
  - chokepoint-capitalism
  - digital-rights-management-critique
  - interoperability-mandates
  coined_by: "Synthesized by Doctorow; draws on platform economics literature and antitrust analysis"
first_appeared: "Synthesized across Doctorow's blog writing and talks, 2019–2023; crystallized in enshittification formulation (2023)"
key_writings: *id001
related_concepts: *id002
coined_by: "Synthesized by Doctorow; draws on platform economics literature and antitrust analysis"
---

The platform decay cycle is the broader lifecycle framework within which [[enshittification]] operates — the arc from open, competitive, user-serving platforms to closed, monopolistic, extractive ones. While enshittification names the specific mechanism of user-to-business-to-shareholder extraction, the platform decay cycle describes the longer structural story: why platforms begin open and end closed, and what prevents correction.

## The Cycle Described

Cory Doctorow's analysis across [[pluralistic-blog]], [[the-internet-con]], and his talks describes a consistent pattern:

**Stage 1: Open and competitive.** A new platform or service enters a market with limited network effects. To attract users, it must offer genuine value. It may embrace openness as a growth strategy — allowing third-party developers, not charging high fees, tolerating adversarial interoperability by competitors. The internet's early web, early Facebook, early Twitter, and early app stores each exhibited some features of this stage.

**Stage 2: Network effects and lock-in.** As the platform grows, it accumulates network effects: users are on the platform because other users are there. [[switching-costs]] rise because users' accumulated social graphs, histories, and content are in the platform's custody. The platform begins investing in technical and legal mechanisms that raise those switching costs further — [[digital-rights-management-critique|DRM]], anti-scraping terms, proprietary formats, API closures.

**Stage 3: Monetization pivot.** With users locked in, the platform pivots its value proposition from "serve users" to "extract from users and business customers." This is the [[enshittification]] stage: the subsidy-then-extraction sequence. Algorithmic feeds are degraded until businesses pay for reach. Advertising fills the product. Organic features are replaced with paid ones.

**Stage 4: Decay and attempted correction.** The platform becomes objectively worse. Users recognize the decay but cannot easily leave — [[adversarial-interoperability]] has been suppressed, data cannot be exported, social graphs are inaccessible to competing services. Regulatory attention may arrive, but structural remedies are slow. The platform may lobby to forestall them.

**Stage 5: Replacement or collapse.** Eventually, a new entrant finds a way to bypass the incumbent's defenses — a new platform paradigm that starts the cycle again, a regulatory intervention that forces interoperability, or simple collapse as users find the platform worthless enough to abandon despite the costs.

## Why the Cycle Repeats

Doctorow's argument is that the cycle repeats because the structural conditions that enable it are not addressed. Each new platform learns from the previous ones and accelerates the lock-in phase. [[self-help-ip]] mechanisms become more sophisticated. Legal infrastructure (DMCA, CFAA) grows more hostile to [[competitive-compatibility]]. The window during which adversarial interoperability might have broken the cycle narrows.

The cycle also repeats because the remedy — [[interoperability-mandates]] — is politically and technically difficult to implement. Incumbents use their market power to resist regulation, and by the time regulatory will exists, the incumbent's position is entrenched.

## Relationship to Other Frameworks

The platform decay cycle is Doctorow's synthesis and extension of several bodies of analysis:

- [[tim-wu]]'s "Cycle" in telecommunications (his 2010 book *The Master Switch*) traces how new communications technologies move from open to closed control — a macro-historical version of the same pattern
- [[lina-khan]]'s Amazon analysis describes the subsidy-then-extraction dynamic in e-commerce specifically
- [[matt-stoller]]'s work on monopoly describes how market power enables the extraction phase

Doctorow's contribution is to synthesize these into a portable framework and connect the diagnosis (monopoly-enabled lock-in) directly to the remedy ([[adversarial-interoperability]] and [[interoperability-mandates]]).

## In Fiction

The platform decay cycle is not merely a theoretical construct in Doctorow's work — it appears as a plot driver in several novels. [[walkaway]] imagines communities that opt out of the dominant platform economy entirely, building open alternatives. [[pirate-cinema]] and [[homeland]] dramatize the lock-in and control aspects of platform power in near-future settings. [[makers]] depicts the creative destruction of legacy industries and the rise of new ones, with attention to how openness enables innovation and how incumbents suppress it.
