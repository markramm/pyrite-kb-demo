---
id: release-of-gpl-v1
title: "Release of GPL v1"
type: event
importance: 8
tags:
- gpl
- license
- copyleft
- 1989
date: 1989-02-01
location: "Cambridge, MA"
participants:
- stallman
- free-software-foundation
significance: "The first version of the GNU General Public License formalized the copyleft mechanism in legally enforceable terms, establishing the template for all subsequent free software licenses."
research_status: draft
---

The first version of the GNU General Public License was released in February 1989, formalizing the [[copyleft]] mechanism that [[stallman]] had been implementing informally in earlier GNU software distributions. Before the GPL, GNU software had been distributed with a notice that was philosophically copyleft but legally informal — it expressed Stallman's intent but was not drafted as an enforceable license. [[gpl-v1]] was the first version written as a proper legal instrument.

The [[gpl-copyleft-mechanism]] as formalized in v1 worked by leveraging copyright: the license granted users the right to copy, modify, and redistribute the software, but only on the condition that any distributed modifications be licensed under the same terms. The mechanism had been described conceptually in the [[gnu-manifesto]], but the GPL turned the concept into executable law. [[eben-moglen]] later described the GPL's logic as using copyright's exclusivity as a lever to guarantee inclusion: the licensor uses the right to exclude in order to ensure no one can be excluded.

GPLv1 addressed two specific problems [[stallman]] had observed: the practice of distributing binaries without source code (addressed by requiring source code availability with any binary distribution), and the practice of attaching additional restrictions to GPL software (addressed by the "no additional restrictions" clause). If a distributor could not comply with the GPL's terms — for example, because a patent license they held imposed restrictions the GPL prohibits — then they could not distribute the software at all.

The release of [[gpl-v1]] is a landmark in the [[founding-gnu-and-fsf-1983-1991]] era. It transformed the [[gnu-project]] from a software project with a philosophy into a software project with a legal framework. The [[gpl-v2]], released two years later, would refine the language; the [[gpl-v3]] would address new threats that hadn't existed in 1989. But the conceptual architecture — copyleft as a viral, self-reinforcing freedom guarantee — was established here.
