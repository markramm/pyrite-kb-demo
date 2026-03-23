---
id: copyleft-as-legal-hack
title: "Copyleft as Legal Hack"
type: note
importance: 8
tags:
- copyleft
- copyright
- legal-strategy
- gpl
- analysis
research_status: draft
---

[[copyleft]] is, at its structural core, an act of intellectual judo: it uses the strongest weapon of proprietary software — copyright's power of exclusion — to guarantee the opposite of what copyright typically guarantees. Ordinarily, copyright gives the author the right to prevent copying. [[stallman]]'s insight was that this right could be deployed not to prevent copying but to prevent the prevention of copying: grant the right to copy, modify, and redistribute, but condition that grant on passing the same rights to all downstream recipients.

The [[gpl-copyleft-mechanism]] is often described as "viral," a term [[stallman]] objects to because it implies contamination. He prefers "reciprocal." The mechanism works because copyright law's enforcement apparatus backs it: a party who distributes modified GPL software without complying with the license's terms is not just violating a community norm — they are infringing copyright, which is actionable. The FSF's copyright assignment requirement (contributors assign copyright to the FSF for FSF-maintained projects) ensures there is a clear rightsholder capable of bringing that action.

The elegance of the hack is that it requires no new law, no new institutions, no government action. It operates entirely within the existing copyright system, using that system's own logic against the outcome the system typically produces. [[stallman]] has described the insight as recognizing that copyright's power is not inherent to its justification — the system claims to incentivize creation, but the exclusivity it creates can equally well be used to guarantee sharing. His essay [[misinterpreting-copyright]] argues that copyright was originally conceived as utilitarian rather than property-based, a historical point that underpins the philosophical legitimacy of the copyleft hack.

This structure influenced everything that came after. [[larry-lessig]]'s [[creative-commons]] used the same mechanism to extend copyleft-style licensing to cultural works; [[eben-moglen]] built his theory of the GPL around the same logic. The [[free-software-influence-on-creative-commons]] note traces that lineage. The [[gpl-v3]] extended the hack by requiring that the legal freedom to modify be accompanied by practical capability (installation information) — recognizing that [[tivoization]] was a new form of restriction that copyright law itself hadn't anticipated.

The hack has limits, and [[stallman]] has been precise about them. Copyright copyleft works only for works subject to copyright. It cannot guarantee hardware freedom (the motivation for the anti-tivoization clause), cannot prevent [[saas-loophole|SaaS loopholes]] without the [[agpl]], and cannot address [[digital-restrictions-management]] imposed at the hardware level. The history of GPL versions is partly the history of discovering where the legal hack doesn't reach and extending it.

One underappreciated aspect of the hack: it works with the grain of developer motivation. Programmers who want their code used widely are incentivized to release it under terms that allow wide use; the copyleft condition then propagates those terms automatically. [[stallman]] designed a system that aligns the individual programmer's interest in broad adoption with the collective interest in software freedom — without requiring programmers to be ideologically committed to that collective interest.
