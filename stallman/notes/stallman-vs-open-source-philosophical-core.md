---
id: stallman-vs-open-source-philosophical-core
title: "Stallman vs. Open Source: Philosophical Core"
type: note
importance: 8
tags:
- open-source
- free-software
- philosophy
- schism
- eric-raymond
- analysis
research_status: draft
---

The [[software-freedom-vs-open-source]] dispute is regularly mischaracterized as a branding disagreement or a personality conflict. It is, at its core, a genuine philosophical difference about the nature of the problem being solved — and [[stallman]]'s precision about this distinction is one of the most carefully maintained positions in his public record.

**Stallman's position:** Software freedom is an ethical imperative. Users of software have a moral right to run, study, modify, and redistribute the programs they use — rights summarized in the [[four-freedoms]] framework. A program that denies these rights wrongs its users, regardless of how convenient or well-made it is. The [[free-software-definition]] is a rights framework, not a quality standard. [[stallman]] explicitly argues, in [[why-open-source-misses-the-point]] and elsewhere, that "open source" is a deliberate evasion: it recasts a rights issue as an engineering methodology, allowing advocates to support "open" development while ignoring the question of user freedom entirely.

**The open source position (as articulated by [[eric-raymond]] and others):** Open development produces better software. When source code is available for inspection and modification by a large distributed community, bugs are found faster, security vulnerabilities are exposed and patched, and development velocity is higher. The [[cathedral-and-bazaar-raymond]] argument is empirical and economic: the bazaar model of open development outcompetes the cathedral model of proprietary development. This position does not require any claim about user rights; it makes a claim about development efficiency.

**Where they agree:** Both positions endorse the major copyleft licenses — the GPL family is both "free software" and "open source" by the respective definitions. Both positions support the same practical outcome (source code available, redistributable, modifiable) in the typical case. The OSI's Open Source Definition and the FSF's [[free-software-definition]] overlap significantly; the major free software licenses are also open source licenses and vice versa.

**Where they diverge:** The divergence becomes visible at the edges. The open source position has no objection to "open core" business models (free community edition, proprietary enterprise additions), because these models can still produce high-quality open components. [[stallman]]'s position objects: open core is a trap that leads users toward proprietary extensions. The open source position has no objection to Tivoized devices that run Linux but prevent modification, because the source is available for inspection. [[stallman]]'s position requires the anti-[[tivoization]] clause of [[gpl-v3]]: the right to modify is meaningless if you can't install your modification. The open source position is silent on [[digital-restrictions-management]] and [[saas-loophole|SaaS loopholes]]; [[stallman]]'s position opposes both as violations of the [[four-freedoms]].

**The strategic consequence:** [[stallman]] argues that the open source movement, by refusing to make the ethical argument, has produced a world where corporations can claim "open source" credentials while systematically restricting user freedom. He points to cloud computing, DRM, and Tivoization as areas where the absence of the ethical argument has allowed freedom to erode. Open source advocates argue that the pragmatic framing has produced far broader corporate adoption and far more open code in the world than the ethical framing would have achieved.

Both positions are internally consistent. The [[free-vs-open-source-schism-1998-2007]] era documents how the divergence became institutionalized; the [[gplv3-and-later-career-2006-present]] era shows [[stallman]] extending the ethical framework to address vulnerabilities the previous decade had revealed.
