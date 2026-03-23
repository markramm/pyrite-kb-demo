---
id: lgpl
title: "GNU Lesser General Public License"
type: writing
importance: 8
tags:
- license
- copyleft
- lgpl
- free-software
- legal
- libraries
writing_type: license-text
date: 1991-06-01
coauthors: []
publication: "Free Software Foundation"
url: "https://www.gnu.org/licenses/lgpl-3.0.html"
key_concepts:
- copyleft
- gpl-copyleft-mechanism
- free-software-definition
research_status: draft
---

The GNU Lesser General Public License (LGPL) — originally named the "Library GPL" when first released alongside [[gpl-v2]] in June 1991 — is a weaker form of [[copyleft]] designed specifically for software libraries. Where the full GPL requires that any derivative work be licensed under the GPL, the LGPL allows proprietary software to link against LGPL-licensed libraries without triggering the copyleft requirement, provided the user retains the ability to replace the library with a modified version.

The strategic rationale for the LGPL reflects a pragmatic tension within [[stallman]]'s thinking. A library licensed under the full GPL would be unusable by proprietary software developers, which would effectively exclude the library from the proprietary software world — and thus from widespread adoption. For libraries where the [[free-software-foundation]] wanted to compete with existing proprietary alternatives, this exclusion would be counterproductive. The LGPL was the compromise: use it for libraries where adoption matters, apply the full GPL where the goal is to insist on a free ecosystem.

[[stallman]] later expressed ambivalence about the LGPL and renamed it from "Library GPL" to "Lesser GPL" in version 2.1 (1999) to emphasize that it offers less protection for software freedom than the full GPL. In his essay on the topic (hosted at gnu.org), he argues that the LGPL should be used only when the tactical benefit of wider adoption outweighs the strategic cost of allowing proprietary software to benefit from free library code without contributing back.

The GNU C Library (glibc) uses the LGPL, which is why proprietary programs can legally run on GNU/Linux systems: they link against glibc without inheriting the GPL. This pragmatic decision by the [[gnu-project]] enabled the commercial Linux ecosystem to exist, but it also means that enormous amounts of proprietary software benefit from the [[gpl-copyleft-mechanism]]'s lesser form without contributing to the free software commons.

The LGPL went through its own versioning: LGPL 2.0 (1991), LGPL 2.1 (1999), and LGPL 3.0 (2007, updated in parallel with [[gpl-v3]]). The 3.0 version adds the [[gpl-v3]]'s anti-[[tivoization]] and patent provisions, though for linking scenarios rather than full program distribution. The [[free-software-foundation]] maintains that LGPL 3.0 is technically structured as an additional permissions document on top of [[gpl-v3]], reflecting a cleaner modular architecture for the GPL license family.
