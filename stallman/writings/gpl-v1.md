---
id: gpl-v1
title: "GNU General Public License, Version 1"
type: writing
importance: 9
tags:
- license
- copyleft
- gpl
- free-software
- legal
writing_type: license-text
date: 1989-02-01
coauthors: []
publication: "Free Software Foundation"
url: "https://www.gnu.org/licenses/old-licenses/gpl-1.0.html"
key_concepts:
- copyleft
- gpl-copyleft-mechanism
- free-software-definition
research_status: draft
---

The first version of the GNU General Public License, released in February 1989, was the first operational implementation of [[copyleft]] as a legal mechanism. It transformed the intuition behind [[gnu-manifesto]] — that software freedom must be preserved through the conditions of distribution — into enforceable license terms. The event [[release-of-gpl-v1]] marks one of the key moments of the [[founding-gnu-and-fsf-1983-1991]] era.

The core mechanism of GPL v1 is what [[stallman]] called "copyleft": using copyright law's grant of exclusive rights to the author in order to guarantee, rather than restrict, the freedoms of users. Anyone who distributes GPL-licensed software must make the source code available and must license any derivative works under the same terms. This "share-alike" condition is the [[gpl-copyleft-mechanism]] in operation.

GPL v1 addressed a specific problem [[stallman]] had encountered: distributors were modifying GNU software into proprietary products by combining it with other code in ways that technically complied with earlier less-formal conditions. The license's "distribution" requirements closed these gaps by requiring that the complete corresponding source code be provided whenever binaries were distributed.

The preamble of GPL v1 is a statement of philosophy as much as a legal recital. It explicitly names the goal: to guarantee "the freedom to share and change free software — to make sure the software is free for all its users." This preamble was drafted with help from [[eben-moglen]], who would become the [[free-software-foundation]]'s general counsel and the primary legal architect of subsequent GPL versions.

GPL v1 covered less territory than its successors. It lacked the patent clauses later added in [[gpl-v2]], and it did not address hardware restrictions ([[tivoization]]) that would be covered in [[gpl-v3]]. But it established the fundamental structure — permissions, conditions, and no-warranty disclaimers — that all subsequent GPL versions and many other copyleft licenses inherit.

The practical impact of GPL v1 was initially limited to the [[gnu-project]]'s own software. The license's wider significance became apparent only when [[linus-torvalds]] chose to release the Linux kernel under GPL v2 in 1992, creating the combination of GNU tools and Linux kernel that [[stallman]] insists should be called [[gnu-linux-naming|GNU/Linux]].
