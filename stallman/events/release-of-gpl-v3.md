---
id: release-of-gpl-v3
title: "Release of GPL v3"
type: event
importance: 8
tags:
- gplv3
- license
- copyleft
- tivoization
- drm
- software-patents
- 2007
date: 2007-06-29
location: "Cambridge, MA"
participants:
- stallman
- eben-moglen
- free-software-foundation
- software-freedom-law-center
significance: "GPLv3 closed the tivoization loophole and added explicit patent retaliation clauses, representing the FSF's response to a decade of new threats to software freedom that GPLv2 had not anticipated."
research_status: draft
---

After the [[gplv3-drafting-process]] — 18 months of public drafting, four discussion drafts, and an unprecedented consultation process involving corporations, civil society organizations, and individual developers worldwide, [[gpl-v3]] was released on June 29, 2007. The process was designed by [[stallman]] and the [[free-software-foundation]], with [[eben-moglen]] and the [[software-freedom-law-center]] as primary legal drafters. The public process was partly principled (the FSF believed its users deserved input into the license they used) and partly strategic (the consultation built legitimacy for changes that some in the open source community were resisting).

The two central innovations addressed problems that had not existed when [[gpl-v2]] was written:

Anti-tivoization: TiVo had shipped Linux-based devices with cryptographic signature checks that prevented users from running modified kernels on the hardware. The modified source code was available under GPLv2's terms, satisfying the letter of the license, but the [[tivoization]] mechanism made the freedom to modify meaningless in practice. GPLv3's "Installation Information" requirement mandates that anyone distributing GPL software on consumer devices must also provide everything necessary to install and run modified versions on those devices. This closes the loophole by requiring that the freedom to modify be practically exercisable, not just theoretically available.

Patent retaliation: GPLv3 contains explicit language terminating the rights of any party that initiates patent litigation against GPL software users. This was directed at the growing use of software patents as weapons against free software, a problem that had intensified during the [[free-vs-open-source-schism-1998-2007]] era.

The most significant political consequence of GPLv3 was [[linus-torvalds]]'s refusal to upgrade the Linux kernel. Torvalds argued the anti-tivoization clause regulated hardware rather than software and that the patent language was too broad. His decision, shared by most kernel maintainers, meant that the Linux kernel and the GNU toolchain became licensed under different GPL versions for the first time. This division has never been resolved.

The release of GPLv3 is the central event of the [[gplv3-and-later-career-2006-present]] era and represents the mature expression of [[stallman]]'s [[gpl-copyleft-mechanism]] theory — a theory that freedom requires not just legal permission but practical capability.
