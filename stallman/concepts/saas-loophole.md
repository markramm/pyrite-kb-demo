---
id: saas-loophole
title: The SaaS Loophole (ASP Loophole)
type: concept
tags:
- saas
- gpl
- copyleft
- legal
- technical
links:
- target: platform-decay-cycle
  relation: related_to
  note: Stallman's SaaS loophole (GPL doesn't cover server-side software) and Doctorow's
    platform decay cycle both describe how control migrates from users to vendors
    over time
  kb: doctorow
- target: enshittification
  relation: related_to
  note: Stallman's identification of the SaaS loophole anticipated the structural
    conditions that enable enshittification. When software runs on someone else's
    server, users have none of the four freedoms, which is precisely what allows platforms
    to degrade service quality without consequence.
  kb: doctorow
importance: 7
concept_type: legal
first_appeared: Identified during GPLv2 era; addressed by AGPL (2002, revised 2007)
key_writings:
- agpl
- gpl-v3
- who-does-that-server-really-serve
related_concepts:
- gpl-copyleft-mechanism
- copyleft
- four-freedoms
- free-software-definition
- software-freedom-vs-open-source
research_status: draft
---

The SaaS loophole (sometimes called the ASP loophole, from "Application Service Provider") is a gap in the [[gpl-v2]]'s [[gpl-copyleft-mechanism]]: a company can take GPL-licensed software, modify it substantially, run it on a server, and provide users access to it as a networked service — all without triggering the GPL's copyleft obligation to distribute the source code of their modifications.

## Why the Gap Exists

The [[gpl-v2]]'s copyleft clause is triggered by **distribution** — providing copies of the software to others. Running software on a server and offering users access to its functionality does not constitute distribution. Users interact with the running software but never receive a copy of it. Therefore, no distribution occurs, and no copyleft obligation arises.

This was not a significant issue when GPLv2 was written in 1991: networked applications were rare, the Web barely existed, and the model of running software remotely and accessing it through a browser was not yet a dominant deployment pattern. By the 2000s, it had become one of the primary ways software was deployed — and the loophole had become significant.

## Practical Consequences

The SaaS model allows companies to:

1. Take GPL-licensed software (a database, a web framework, a content management system).
2. Modify it heavily to create a proprietary service.
3. Offer that service commercially.
4. Never release the source code of their modifications.

This is not copyright infringement — it is entirely within the GPL's terms. But it produces an outcome contrary to the GPL's spirit: valuable improvements to free software are locked inside proprietary services and never returned to the community.

[[stallman]]'s essay [[who-does-that-server-really-serve]] (2010) addresses this directly: when you use a web service, you do not control the software running it. The server may be running free software internally, but you have none of the [[four-freedoms]] with respect to it — you cannot study it, modify it, or redistribute it.

## The AGPL Response

The [[agpl]] (Affero GPL) was created specifically to close this loophole. The Affero GPL v1 was created by Affero Inc. in 2002 for their online community software. The [[free-software-foundation]] later produced the AGPLv3 (2007) as a companion to [[gpl-v3]].

The AGPLv3 adds a network-use trigger: if you run a modified version of AGPLv3-licensed software on a server that users interact with over a network, you must make the source code of your modified version available to those users. This extends copyleft to the SaaS deployment model.

The AGPL is not the same as GPLv3; it is a separate license. Code under AGPLv3 cannot be freely mixed with code under GPLv3 without triggering the AGPL's requirements for the combined work (unless explicitly permitted).

## Adoption and Resistance

The AGPL has been adopted by several prominent free software projects: MongoDB (though MongoDB later switched to a non-free license), GNU Social, Mastodon (ActivityPub implementation), and others. Some companies have explicitly prohibited the use of AGPL-licensed software in their products precisely because it closes the loophole they rely on.

[[stallman]] recommends the AGPL for any software likely to be deployed as a networked service. The [[free-software-foundation]]'s position is that AGPL is the correct copyleft license for server software; GPLv3 is appropriate for programs that users run on their own machines.

## Unresolved Tension

Closing the SaaS loophole raises its own questions about the scope of copyleft. The standard GPL logic is: if you distribute, you must share your changes. The AGPL extends this to: if you provide a service using the software, you must share your changes. But this creates a new boundary question: what counts as "providing a service" to users? Private use within a company? A service for employees? A service with one user?

The AGPL's answer — network interaction that makes the software's functionality available to external users — is pragmatic but not philosophically airtight. [[stallman]] acknowledges these edge cases but regards the AGPL's core principle as correct: users who depend on a server's software should have access to that software.
