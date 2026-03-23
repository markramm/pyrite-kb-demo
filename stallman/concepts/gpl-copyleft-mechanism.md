---
id: gpl-copyleft-mechanism
title: The GPL's Copyleft Mechanism
type: concept
tags:
- gpl
- copyleft
- legal
- technical
- licensing
links:
- target: competitive-compatibility
  relation: related_to
  note: GPL's copyleft mechanism enforces interoperability of derivatives; Doctorow's
    competitive compatibility argues for similar structural openness to prevent lock-in
  kb: doctorow
importance: 9
concept_type: legal
first_appeared: gpl-v1 (1989)
key_writings:
- gpl-v1
- gpl-v2
- gpl-v3
- lgpl
- agpl
related_concepts:
- copyleft
- four-freedoms
- tivoization
- saas-loophole
- free-software-definition
research_status: draft
---

The GPL's copyleft mechanism is the legal engine that makes [[copyleft]] self-enforcing. Understanding it requires distinguishing the philosophical goal (keeping software free) from the legal technique (conditions attached to copyright permissions). The mechanism has three interacting elements: the grant of permissions, the copyleft condition, and the distribution trigger.

## The Grant of Permissions

Copyright law gives the author exclusive rights to copy, distribute, and create derivative works. Without a license, any of these acts by another party is infringement. The GPL begins by granting broad permissions: you may copy, distribute, and modify the program. This is what makes GPL software usable by anyone.

## The Copyleft Condition

The permissions come with a condition: if you distribute a covered work — in source or binary form — you must distribute it under the GPL, and you must provide or offer the complete corresponding source code. This condition is attached to the act of distribution, not to the act of modification or internal use.

The legal formulation in [[gpl-v2]] Section 2 says: you may distribute modifications, "provided that you also meet all of these conditions" — including that the work "be licensed as a whole... to all third parties under the terms of this License." The key legal word is "provided" — permissions are granted on these conditions, not unconditionally.

This structure is why the GPL does not function as a contract in the traditional sense. It is a unilateral grant of copyright permissions subject to conditions. Failure to comply with the conditions does not breach a contract; it simply means the permissions were never validly granted, and distribution without permission is copyright infringement. [[eben-moglen]] developed the formal legal argument for this understanding, which prevailed in the major GPL enforcement cases.

## The Distribution Trigger

The copyleft condition is triggered by **distribution** — providing copies to others. It is not triggered by modification alone, or by use, or by running software on a server for users to interact with. This last gap is the [[saas-loophole]]: a company can modify GPL software and run it as a service without distributing it, thus incurring no copyleft obligation. The [[agpl]] closes this gap by adding a network-use trigger.

What counts as distribution is thus a critical question. The GPL does not define it explicitly; courts and the FSF have interpreted it to mean conveying copies of the software to parties outside your organization. Internal use — including within a corporation — does not trigger copyleft.

## Derivative Works and Linking

The most contested aspect of the GPL mechanism is the question of what constitutes a "derivative work" requiring GPL compliance. The GPL covers not just modified versions of a program but works "based on" it. In the software context, this raises questions about:

- **Static linking**: A program compiled with GPL library code statically linked in is generally considered a derivative work requiring GPL compliance.
- **Dynamic linking**: A program that calls a GPL library at runtime through a shared library interface — the [[lgpl]] was specifically designed to permit this without triggering strong copyleft.
- **Aggregation**: Multiple programs distributed together on the same medium are not automatically derivatives of each other. The GPL explicitly distinguishes between a combined work and "mere aggregation."

The [[free-software-foundation]]'s position is that dynamic linking to a GPL library generally creates a derivative work. This position is disputed by some lawyers and is not definitively settled by case law, but it is the FSF's interpretation and guides its enforcement practice.

## Evolution Across GPL Versions

[[gpl-v1]] (1989) established the basic mechanism. [[gpl-v2]] (1991) refined it, adding the "liberty or death" clause (Section 7): if copyright law or patents prevent you from distributing GPL software under its terms, you may not distribute it at all. This prevents a scenario where a distributor encumbers GPL code with patent licenses that restrict recipients.

[[gpl-v3]] (2007) added two major mechanical extensions:

1. **Anti-tivoization**: Section 6 requires that users who receive object code for a "user product" (a consumer device) receive the information necessary to install modified versions on that device. This addresses [[tivoization]] — hardware that runs only manufacturer-signed binaries.

2. **Patent peace**: Section 11 requires GPL distributors to grant all downstream recipients a patent license for any patents they hold that cover the distributed code. This addresses the threat of "submarine patents" in distributed software.

## Enforcement

The GPL is enforced as a copyright license. The [[software-freedom-conservancy]] (successor to the FSF's enforcement work) and [[eben-moglen]] at the [[software-freedom-law-center]] have pursued GPL compliance through litigation and negotiation. The key cases (Busybox litigation in the US, GPL enforcement cases in Germany) established that the GPL is a valid copyright license, enforceable against distributors who fail to provide source code.

[[stallman]]'s position has always been that the GPL's purpose is compliance, not punishment — the goal is to get source code released, not to win damages. This has shaped FSF enforcement philosophy: seek compliance first, litigation as a last resort.
