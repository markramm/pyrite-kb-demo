---
id: software-patents-opposition
title: Opposition to Software Patents
type: concept
tags:
- software-patents
- legal
- policy
- advocacy
- strategic
links:
- target: adversarial-interoperability
  relation: related_to
  note: Stallman's software patent opposition and Doctorow's adversarial interoperability
    both identify IP law weaponization as the key threat to open software ecosystems
  kb: doctorow
importance: 8
concept_type: strategic
first_appeared: Stallman began writing on software patents in the early 1990s; formal
  campaign through League for Programming Freedom (1989)
key_writings:
- free-software-free-society
- why-software-should-be-free
- gpl-v3
related_concepts:
- four-freedoms
- copyleft
- gpl-copyleft-mechanism
- digital-restrictions-management
- free-software-definition
research_status: draft
---

[[stallman]]'s campaign against software patents is one of the longest-running threads in his activism — predating even the mature [[copyleft]] framework and continuing to the present. His position is categorical: software should not be patentable, because software patents restrict programming in ways that copyright does not and that serve no legitimate social purpose.

## The Core Argument

Patent law grants inventors a time-limited monopoly over the use of an invention in exchange for public disclosure. The rationale is that patents encourage disclosure (rather than trade secrecy) and provide investment incentives for expensive research and development.

[[stallman]]'s argument is that software does not fit this rationale:

1. **Software is mathematical**: Programs are implementations of mathematical algorithms. Patenting software is equivalent to patenting mathematical procedures, which courts in most jurisdictions have historically refused.

2. **No disclosure benefit**: Software development does not depend on patent protection to incentivize disclosure. The norms of the software industry — open publication of techniques, conference presentations, the academic CS literature — were well established before software patents became common. Disclosure happens without the patent incentive.

3. **Development cost is low compared to hardware**: The patent system was designed for hardware inventions requiring large capital investment. A programmer can implement a patented technique in days or weeks without knowing the patent exists. Patent exposure is proportional to productivity.

4. **Software patents create a minefield**: The [[free-software-foundation]] and League for Programming Freedom documented cases where simple, obvious software techniques were patented — GIF compression (LZW algorithm), MP3 encoding (various codec patents), one-click shopping (Amazon). Any substantial program is likely to implement dozens of techniques that someone, somewhere, has patented.

## The League for Programming Freedom

[[stallman]] co-founded the League for Programming Freedom in 1989, specifically to campaign against both software patents and interface copyrights (a separate threat that emerged from the "look and feel" lawsuit era). The League predates the FSF's formal anti-software-patent campaign and was Stallman's first organized advocacy effort outside of the free software licensing framework.

## Impact on the GPL

Software patents interact dangerously with [[copyleft]]: a patent holder can grant a patent license for a GPL program while attaching conditions that restrict downstream distribution — effectively undermining the GPL. [[gpl-v2]]'s Section 7 (the "liberty or death" clause) addresses this by saying that if a GPL distributor cannot comply with both the patent license and the GPL, they may not distribute at all. This prevents the use of patent licenses as a mechanism for injecting restrictions into GPL software.

[[gpl-v3]] goes further with Section 11, requiring GPL distributors to grant all downstream recipients a license under any patents they hold that cover the distributed code. This is the "patent peace" provision.

## The EU Software Patents Battle

In the early 2000s, the European Commission proposed a directive that would have permitted software patents in the EU (which had largely resisted them under European Patent Office practice). [[stallman]] campaigned actively against this proposal, arguing it would import the US software patent problem into Europe. The directive was rejected by the European Parliament in 2005 in a rare legislative defeat for a Commission proposal — a victory that [[stallman]] and the [[free-software-foundation]] claimed as significant.

## Alice and Recent Developments

The US Supreme Court's 2014 decision in Alice Corp. v. CLS Bank significantly restricted software patent eligibility in the United States, invalidating patents on abstract ideas implemented on generic computer hardware. [[stallman]] welcomed this as a step in the right direction while arguing that the ruling did not go far enough — software should be categorically excluded from patentability.

## Relationship to Other Campaigns

Software patents are one of three major legal threats [[stallman]] has consistently identified: proprietary licensing (addressed by the GPL), software patents (addressed by advocacy and GPL patent provisions), and [[digital-restrictions-management]] (addressed by [[gpl-v3]] and advocacy). All three share a common structure: legal or technical mechanisms that prevent users from exercising the [[four-freedoms]].
