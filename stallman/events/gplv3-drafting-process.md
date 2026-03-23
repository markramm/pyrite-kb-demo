---
id: gplv3-drafting-process
title: "GPLv3 Drafting Process (2006–2007)"
type: event
tags:
- gplv3
- drafting
- public-consultation
- tivoization
- drm
- patents
links:
- target: crypto-wars-export-controls
  relation: related_to
  note: The GPLv3 drafting process and the Crypto Wars represent parallel struggles over whether governments and corporations can restrict users' control over software on their own machines. Both turned on the principle that user control over their own computing is a right.
  kb: schneier
importance: 9
date: 2006-01-01
location: "Cambridge, MA (FSF); international public process"
participants:
- stallman
- eben-moglen
- free-software-foundation
- linus-torvalds
---

The drafting of [[gpl-v3]] ran from January 2006 through its release on June 29, 2007 — an unprecedented eighteen-month public consultation process that produced four public drafts and solicited comments from thousands of individuals and organizations worldwide. The process was organized by the [[free-software-foundation]] and led by [[stallman]] with [[eben-moglen]] as the primary legal architect.

The drafting addressed three major technical and legal problems that had emerged since [[gpl-v2]] was released in 1991.

The first was [[tivoization]]: TiVo and similar hardware manufacturers had used GPL-licensed software in products whose hardware was locked down so that users could not actually install modified versions of the software, even though the GPL's source-code requirements were technically satisfied. Stallman argued this violated the spirit of the [[four-freedoms]] — freedom to modify is hollow if the hardware prevents running the modification. GPLv3 added the "Installation Information" requirement to close this loophole.

The second was [[digital-restrictions-management]]: GPLv3 prohibited using GPL-covered software as part of effective technological protection measures in ways that restrict users. This was controversial; some argued it made the GPL incompatible with legitimate security applications, while Stallman maintained the distinction between security and control.

The third was software patents: GPLv3 included an explicit patent retaliation clause and addressed the risk of patent cross-licensing deals (such as the Microsoft-Novell agreement of 2006) being used to fragment the free software ecosystem.

[[linus-torvalds]] publicly and consistently opposed GPLv3 throughout the drafting process, objecting to the tivoization provisions and the complexity of the new license. He announced that the Linux kernel would remain under [[gpl-v2]] only, a decision that stood. This created a permanent bifurcation: the [[gnu-project]]'s tools and the FSF-maintained software moved to GPLv3, while Linux remained on GPLv2-only. The [[gnu-linux-naming]] controversy acquired a new layer: the two halves of the system were now under different GPL versions with different philosophical commitments.

The public drafting process itself was significant as a model of open governance. Comments from the public, legal scholars, and industry were incorporated into successive drafts, documented on the gplv3.fsf.org site. This transparency was partly a deliberate contrast with the closed processes of proprietary licensing. The resulting license is longer and more technically complex than GPLv2, reflecting the more sophisticated legal environment four decades into the software industry's development.

The [[gplv3-and-later-career-2006-present]] era is defined in large part by the consequences of this process: the split with Torvalds over tivoization, the [[saas-loophole]] that GPLv3 still did not close (addressed later by the [[agpl]]), and the ongoing debates about whether copyleft can keep pace with new forms of software deployment.
