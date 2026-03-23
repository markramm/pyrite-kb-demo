---
id: copyleft
title: "Copyleft"
type: concept
importance: 9
concept_type: legal-innovation
first_appeared: "gnu-manifesto-1983"
key_writings:
- free-software-free-society-2002
- cathedral-and-the-bazaar-1997
related_concepts:
- four-freedoms
- open-source-definition
- forking-as-governance
tags:
- copyleft
- licensing
- gpl
- stallman
- legal-mechanism
research_status: draft
---

Copyleft is the legal mechanism that transformed the [[four-freedoms]] from a philosophical position into an enforceable condition of software distribution. The concept is covered in depth in the Stallman KB; this entry focuses on copyleft's specific role within the FOSS movement: making the GPL enforceable, anchoring the copyleft-versus-permissive strategic tension, and the long-term shift in copyleft adoption.

The core innovation is a hack on copyright law. Rather than abandoning copyright (which would place software in the public domain and allow anyone to make proprietary derivatives), copyleft uses copyright to impose conditions: you may use, modify, and distribute the software, but any derivative work you distribute must carry the same license. [[richard-stallman]] and the [[free-software-foundation]] embodied this principle in the GPL family of licenses. [[gpl-v2]] (1991) was the first legally robust implementation and became the most widely deployed copyleft license in history, governing the Linux kernel and thousands of other projects. [[lgpl]] offered weak copyleft for libraries, permitting proprietary programs to link against LGPL code without triggering full copyleft. [[gpl-v3]] (2007) extended the mechanism to address hardware restrictions (anti-tivoization) and software patents. [[agpl]] closed the network-use loophole, requiring source disclosure when users interact with modified software over a network.

The copyleft-versus-permissive tension is one of the defining strategic debates in the FOSS movement. From the free software perspective, permissive licenses like [[mit-license]] and [[apache-license-2]] fail to protect downstream users: a corporation can take permissively licensed code, modify it, and release the result as proprietary software, denying users the freedoms the original author intended to guarantee. Copyleft prevents this by making freedom a condition that propagates through the supply chain. From the open source pragmatist perspective, copyleft's restrictions limit corporate adoption and create legal compliance burdens that discourage participation. The [[open-source-definition]] certifies both copyleft and permissive licenses as "open source," but the philosophical tension between them is never resolved — it is the central fault line of [[software-freedom-vs-open-source]].

The adoption trajectory tells a story of shifting strategic preferences. Through the 2000s, copyleft licenses — particularly [[gpl-v2]] — dominated FOSS licensing by project count. The GPL was the default choice for new projects; it carried the cultural weight of the free software tradition and the practical example of Linux. Beginning in the late 2000s and accelerating through the 2010s, permissive licenses overtook copyleft in new project adoption. By the early 2020s, the [[mit-license]] was the most commonly chosen license on GitHub, and [[apache-license-2]] dominated corporate open source projects. Multiple factors drove this shift: the rise of GitHub and its permissive-license defaults; corporate open source programs that preferred permissive licenses for legal simplicity; the JavaScript/npm ecosystem's strong MIT convention; and a generational shift in which new developers encountered open source through corporate-sponsored projects rather than through the free software tradition. The [[gpl-v3]]'s failure to capture the Linux kernel — [[linus-torvalds]] and the kernel maintainers refused to adopt it — was symbolically significant: the most important copyleft project in existence declined to move to the latest copyleft license.

Copyleft remains strategically important even as its adoption share has declined. The AGPL-as-business-model pattern — releasing server software under [[agpl]] to prevent cloud providers from offering it as a managed service without contributing back — became a significant commercial strategy in the [[modern-foss-and-sustainability-crisis-2015-present]] era. The [[sspl-bsl]] controversy tested copyleft's outer boundaries: MongoDB's SSPL attempted to extend copyleft conditions so far that the [[open-source-initiative]] and [[free-software-foundation]] both declined to recognize the license. The copyleft principle itself — that the legal mechanism of copyright can be turned to serve freedom rather than restrict it — remains [[richard-stallman]]'s most durable contribution to the movement, even as the specific licenses that embody it face competitive pressure from permissive alternatives.
