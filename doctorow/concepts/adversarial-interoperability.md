---
id: adversarial-interoperability
title: "Adversarial Interoperability"
type: concept
tags:
- interoperability
- digital-rights
- antitrust
- platform-power
- coined-by-doctorow
links:
- target: four-freedoms
  relation: builds_on
  note: Doctorow's adversarial interoperability defends in practice what Stallman's four freedoms specify in principle — the right to study, modify, and redistribute
  kb: stallman
- target: gpl-v3
  relation: related_to
  note: GPLv3's anti-tivoization and anti-DRM clauses are early legal interoperability mandates — structurally what Doctorow advocates through policy
  kb: stallman
- target: yesterday-s-tomorrow
  relation: related_to
  note: Agre's 1998 analysis of winner-take-all standards competition and network effects provides the structural context for why adversarial interoperability matters
  kb: red-rock-eater
- target: hacking-as-systems-subversion
  relation: related_to
  note: Adversarial interoperability is systems subversion applied to platform lock-in — using existing technical affordances to break monopoly control
  kb: schneier
importance: 9
metadata:
  first_appeared: "Electronic Frontier Foundation blog posts, 2019; developed in subsequent EFF white papers and pluralistic-blog"
  key_writings: &id001
  - pluralistic-blog
  - the-internet-con
  - information-doesnt-want-to-be-free
  related_concepts: &id002
  - competitive-compatibility
  - interoperability-mandates
  - switching-costs
  - enshittification
  - digital-rights-management-critique
  - end-to-end-principle
  coined_by: "Cory Doctorow (coined the term; the practice it names has a longer history)"
first_appeared: "Electronic Frontier Foundation blog posts, 2019; developed in subsequent EFF white papers and pluralistic-blog"
key_writings: *id001
related_concepts: *id002
coined_by: "Cory Doctorow (coined the term; the practice it names has a longer history)"
---

Adversarial interoperability is Cory Doctorow's term for the practice of making a product or service work with a competitor's product without the competitor's permission or cooperation — and against the competitor's active attempts to prevent it. The "adversarial" qualifier distinguishes the practice from cooperative interoperability (where companies agree on shared standards) and from mere compatibility (where products happen to work together).

The concept became central to Doctorow's framework for how digital markets became concentrated and how that concentration might be reversed.

## Definition and Scope

Adversarial interoperability covers a wide range of practices:

- **Reverse engineering** competitors' file formats, protocols, or APIs to enable compatibility
- **Interoperating with live services** by scraping, emulating, or connecting to platforms without permission
- **Creating bridge tools** that allow users to move data between incompatible systems
- **Building on top of** a dominant platform to offer users an alternative while preserving their existing network connections

Doctorow's key insight is that adversarial interoperability was historically a normal feature of competitive technology markets — and that its suppression is a relatively recent development enabled by intellectual property law and technical lock-in mechanisms.

## Historical Examples

Doctorow grounds the concept in concrete history. Early Microsoft Word grew by reading WordPerfect files. Lotus 1-2-3 was displaced partly because competitors reverse-engineered its keyboard commands. Early internet services competed by building on top of each other without permission. VisiCalc lost to Lotus because Lotus could read VisiCalc files; Lotus lost to Excel partly because Excel could read Lotus files.

In each case, an incumbent's market dominance was disrupted not by building a better product in isolation but by connecting to the incumbent's user base — taking their data and social connections with them to the competitor. This dynamic, Doctorow argues, is what made technology markets competitive.

## Why It Matters Now

Doctorow's argument, developed extensively on [[pluralistic-blog]] and in [[the-internet-con]], is that today's platform monopolies — Google, Amazon, Apple, Meta — have successfully suppressed adversarial interoperability through a combination of:

- **Terms of service** that prohibit reverse engineering
- **Digital rights management** (see [[digital-rights-management-critique]]) that makes circumvention illegal under laws like the DMCA
- **Computer fraud statutes** (the CFAA in the US) that criminalize unauthorized access to computer systems
- **Patent thickets** around interface technologies

The result is that the historical mechanism by which market entrants could challenge incumbents has been legally blocked. [[switching-costs]] have risen dramatically. Users who want to leave Facebook cannot take their social graph with them; users who want to leave Amazon cannot take their purchase history. This, Doctorow argues, is not a natural feature of digital markets but a legal and political achievement by incumbents.

## Relationship to Other Concepts

Adversarial interoperability is Doctorow's preferred term for the practice; [[competitive-compatibility]] is the term he sometimes uses interchangeably, with slightly different emphasis (see that entry). The distinction is partly rhetorical: "adversarial" foregrounds the political and legal conflict, "competitive compatibility" foregrounds the market outcome.

[[interoperability-mandates]] represent the policy prescription: if voluntary adversarial interoperability is being suppressed, government mandates could require platforms to expose interfaces. Doctorow treats adversarial interoperability and interoperability mandates as complementary tools.

The concept connects to [[end-to-end-principle]] thinking: a network architecture that keeps the network neutral and pushes intelligence to the edges naturally enables adversarial interoperability; an architecture that centralizes control blocks it.

[[enshittification]] is partly the story of what happens in the absence of adversarial interoperability — lock-in enables the extraction sequence.

## Adoption

The term was taken up by [[electronic-frontier-foundation]] in policy advocacy and has been used in regulatory discussions in the EU (Digital Markets Act) and US contexts. [[lina-khan]]'s FTC explored interoperability requirements in platform markets, and Doctorow's framing influenced how advocates described the problem. [[tim-wu]] and [[zephyr-teachout]] have engaged with similar arguments about interoperability as a competition tool.
