---
id: bsd-license
title: "BSD License"
type: license
importance: 6
license_type: permissive
author: "University of California, Berkeley"
date: 1988-01-01
spdx_id: "BSD-3-Clause"
key_provisions:
- "Redistribution in source and binary form permitted with copyright notice preserved"
- "Original 4-clause version included advertising clause requiring acknowledgment in advertising"
- "3-clause 'New BSD' (1999): advertising clause removed"
- "2-clause 'Simplified BSD': further removes non-endorsement restriction"
related_licenses:
- mit-license
- apache-license-2
- gpl-v2
tags:
- permissive
- berkeley
- unix
- academic
- advertising-clause
research_status: draft
---

One of the earliest FOSS licenses, developed at the University of California, Berkeley in connection with the BSD Unix operating system. The BSD License family exemplifies permissive licensing and has a complicated history shaped by its "advertising clause" controversy, which led to multiple incompatible variants.

## Origins in BSD Unix

BSD Unix (Berkeley Software Distribution) was developed at UC Berkeley through the 1970s and 1980s, building on and extending AT&T's Unix. The BSD software was distributed under a license that permitted broad reuse: recipients could use, modify, and redistribute the software, including in commercial products, as long as they retained the copyright notice.

The BSD tradition predates the FOSS movement's explicit formation. Like the [[mit-license]], it represents research-university sharing norms rather than a theory of software freedom. BSD Unix was a direct ancestor of the modern Internet infrastructure — much of the TCP/IP stack, many network utilities — and its license terms enabled commercial adoption that built the early internet.

## The Advertising Clause Problem

The original 4-clause BSD License required that all advertising materials for products using BSD software include an acknowledgment of UC Berkeley. As BSD code spread into many products, each with its own BSD-licensed components, this created a combinatorial explosion: a product using many BSD-licensed components would need advertising text acknowledging each separately. The FSF identified this as a GPL-incompatibility: the advertising clause imposed an additional requirement that the GPL explicitly prohibited.

In 1999, UC Berkeley relicensed its BSD code under the 3-clause "New BSD" license, dropping the advertising clause. The change resolved the GPL-incompatibility but also revealed how the BSD family had fragmented: many projects still used the 4-clause version, and the variants remained technically distinct licenses.

The 2-clause "Simplified BSD" (also called the "FreeBSD License") further removed the non-endorsement clause, leaving only the requirement to retain copyright and permission notices.

## Strategic Position

The BSD licenses occupy the same permissive territory as [[mit-license]] — both permit proprietary derivative works, both are corporate-friendly, both achieve maximum adoption at the cost of not preserving downstream freedom. The practical difference between MIT and BSD-3-Clause is minimal; the choice often reflects ecosystem convention rather than principled distinction.

From the free software tradition, both suffer the same limitation: they enable the "embrace and extend" dynamic where a company takes permissively licensed code, makes proprietary improvements, and denies users access to those improvements. The [[gpl-v2]]'s [[copyleft]] was specifically designed as an alternative to this outcome.

BSD-licensed code (particularly from the BSDs: FreeBSD, NetBSD, OpenBSD) influenced Apple's Darwin/macOS kernel and many commercial Unix derivatives — demonstrating both the adoption success and the freedom-preservation failure from the copyleft perspective.
