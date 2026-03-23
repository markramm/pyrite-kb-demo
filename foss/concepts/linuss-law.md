---
id: linuss-law
title: "Linus's Law"
type: concept
importance: 6
concept_type: principle
first_appeared: "cathedral-and-the-bazaar-1997"
key_writings:
- cathedral-and-the-bazaar-1997
related_concepts:
- bazaar-model
- forking-as-governance
tags:
- raymond
- torvalds
- bug-finding
- many-eyes
- security
research_status: draft
---

"Given enough eyeballs, all bugs are shallow." Named by [[eric-raymond]] after [[linus-torvalds]], formulated in [[cathedral-and-the-bazaar-1997]]. The claim: with a sufficiently large base of beta-testers and co-developers, every problem will be transparent to someone. Someone will spot the bug, and someone else — or the same person — will understand how to fix it. This inverts the cathedral assumption that software complexity requires restricted access and controlled development.

Raymond's formulation rests on a probabilistic argument. In a closed development model, the number of people who see the code before release is small, and the probability that any given bug will be obvious to one of those few people is correspondingly low. In the bazaar model, where code is released early and often (see [[release-early-release-often]]) and users are treated as co-developers, the number of eyes examining the code is vastly larger. For any particular bug, the probability that at least one person in the community has the specific expertise to recognize and diagnose it increases dramatically. Raymond distinguished between "finding" a bug and "understanding" it, arguing that the hard part of debugging is not fixing but characterizing — and that a large, diverse community dramatically reduces the time to characterization. The law provided the theoretical basis for the [[bazaar-model]]'s claim to engineering superiority over closed development.

The law describes a real effect. Large open source projects do find and fix certain classes of bugs faster than comparable closed-source projects, and the mechanism Raymond described — diverse expertise applied to visible code — is genuine. The Linux kernel's development history provides considerable evidence: thousands of contributors reviewing patches catch errors that any small team would miss. The effect is strongest for functional bugs — incorrect behavior that a user or developer encounters during normal use — where the symptom is visible and the cause, once examined, is legible to someone with the right background.

The law's scope is far more limited than its confident formulation suggests, and the [[xz-backdoor-2024]] provided the most dramatic demonstration of those limits. The xz Utils backdoor was inserted by a social engineering attack that exploited a burned-out solo maintainer's need for help. The malicious code was hidden in binary test data files and injected through the build system — not in the primary source code where "many eyes" might plausibly look. The backdoor went undetected for months and was discovered not by code review but by a performance anomaly noticed by a single engineer. The incident revealed several categories where Linus's Law does not apply: adversarial insertion (where the "bug" is designed to evade review), build infrastructure and test fixtures (which attract far less scrutiny than primary source), social engineering (where the attack surface is human trust, not code), and single-maintainer projects (where the "many eyeballs" simply do not exist). The law works for accidental bugs in visible code; it does not work for deliberate backdoors in overlooked infrastructure maintained by isolated individuals.

Linus's Law remains a useful description of one genuine advantage of open development — the bug-finding power of a large, diverse community — but it is not the security guarantee it is sometimes taken to be. The law's rhetorical power in the [[open-source-schism-and-dotcom-1998-2004]] era, when it helped make the case for corporate adoption of open source, may have contributed to a false sense of security about open source software's reliability. The reality is more nuanced: many eyes help, but only when they are actually looking, and only for the kinds of problems that examination can reveal.
