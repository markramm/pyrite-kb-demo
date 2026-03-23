---
id: gpl-v3
title: "GNU General Public License, Version 3"
type: writing
importance: 9
tags:
- license
- copyleft
- gpl
- free-software
- legal
- tivoization
- patents
- drm
writing_type: license-text
date: 2007-06-29
coauthors: []
publication: "Free Software Foundation"
url: "https://www.gnu.org/licenses/gpl-3.0.html"
key_concepts:
- copyleft
- gpl-copyleft-mechanism
- tivoization
- software-patents-opposition
- digital-restrictions-management
research_status: draft
---

GNU General Public License Version 3, released June 29, 2007 after an eighteen-month public consultation process, represents [[stallman]]'s and [[eben-moglen]]'s most ambitious attempt to close the loopholes that technology had opened in the GPL v2 framework. The event [[release-of-gpl-v3]] marks the culmination of the [[gplv3-and-later-career-2006-present]] era's initial phase. It addresses two problems that [[gpl-v2]] could not anticipate: [[tivoization]] and software patents.

[[tivoization]] — named after TiVo's practice — refers to the use of hardware cryptographic signing to prevent users from running modified versions of GPL-licensed software on devices they own. TiVo shipped Linux (GPL v2) on its set-top boxes but used hardware-level signature verification to ensure that only TiVo-signed binaries would boot. This technically complied with GPL v2 (source code was provided) while completely defeating its purpose (users could not actually run modified software). GPL v3's "anti-tivoization" clause, section 6, requires that when software is distributed in a "user product," the distributor must provide the installation information needed to actually run modified versions.

The patent clauses in GPL v3 (section 11) address a different threat: the possibility that a company could contribute to a GPL project while holding patents that, when asserted, would prevent others from exercising the GPL's freedoms. The clause provides an implicit patent license from any contributor and includes a "patent retaliation" provision: if a licensee initiates patent litigation against another licensee over the covered software, the patent license terminates.

GPL v3 also modernized the license's approach to compatibility with other free software licenses and added provisions addressing [[digital-restrictions-management]] (DRM), which [[stallman]] consistently calls "Digital Restrictions Management." The license prohibits adding DRM restrictions to GPL v3 software, on the grounds that DRM is fundamentally incompatible with user freedom.

The consultation process for GPL v3, organized by [[eben-moglen]] and [[bradley-kuhn]] at the [[software-freedom-law-center]], was the most open and participatory license drafting process in free software history. Four draft versions were released for public comment, with comments from companies, developers, and organizations worldwide.

The aftermath was disappointing from [[stallman]]'s perspective. [[linus-torvalds]] refused to upgrade the Linux kernel from GPL v2, citing objections to the anti-tivoization provisions and skepticism about the patent clauses. This means the Linux kernel — the most widely deployed piece of GPL-licensed software — uses GPL v2-only, while GNU userland tools generally moved to GPL v3. The copyleft ecosystem thus split: GNU/Linux systems contain a mix of GPL v2 and GPL v3 components that cannot be merged.

[[larry-lessig]] at [[creative-commons]] noted the parallel between GPL v3's approach and CC's own license versioning challenges, and both organizations ultimately drew on the other's experience.
