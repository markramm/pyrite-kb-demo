---
id: pre-devops-convergence
title: "Pre-DevOps Convergence (2001-2009)"
type: era
importance: 7
tags:
- infrastructure-automation
- agile
- web-operations
- cfengine
- puppet
date_range: "2001-2009"
key_figures:
- mark-burgess
- gene-kim
- andrew-clay-shafer
key_writings:
- visible-ops-handbook
- continuous-delivery-book
key_concepts:
- infrastructure-as-code
- promise-theory
key_events:
- agile-infrastructure-bof-2008
---

The period before "DevOps" existed as a term. Multiple parallel streams were converging toward the movement, though no one had yet named what they were building toward.

**The Agile stream.** The Agile Manifesto (2001) catalyzed a transformation in software development practice. Through this era, Agile methodologies — Scrum, XP, Kanban — matured and spread. But the Agile community was focused almost exclusively on development. Operations was a separate world, organized around stability, change management, and ITSM frameworks like ITIL. The gap between how developers worked and how operations worked was structural and growing.

**The infrastructure automation stream.** [[mark-burgess]] developed CFEngine starting in 1993 — far earlier than the DevOps movement proper. His subsequent work on [[promise-theory]] (2004-2005) provided a theoretical foundation for declarative [[infrastructure-as-code]]: systems described in terms of desired state rather than imperative commands. Puppet (2005) and Chef (2009) built on this conceptual ground. By 2008, the tooling existed to treat infrastructure programmatically, but the organizational and cultural frameworks for doing so were still forming.

**The web operations stream.** Companies like Google, Amazon, Flickr, and the early web-native companies were operating at scales that broke conventional IT practices. Web operations became a recognizable discipline — people who understood both systems and software, who ran distributed services in production, who had to ship fast and stay up. This community developed practices and culture that had no established name yet.

**The Visible Ops contribution.** [[gene-kim]]'s [[visible-ops-handbook]] (2004) approached the problem from the ITSM side, showing how high-performing IT organizations controlled change while maintaining stability. It was prescient about what would later be formalized as DevOps principles — but framed for enterprise operations audiences rather than the Agile development community.

**The convergence moment.** The [[agile-infrastructure-bof-2008]] at the Agile Conference in Toronto was the pivot. [[andrew-clay-shafer]] had been developing the concept of "Agile Infrastructure" — applying Agile principles to operations. Only one person showed up to his Birds of a Feather session: [[patrick-debois]], a Belgian consultant who had been frustrated by the dev-ops divide on his own projects. That conversation planted the seed for what became DevOpsDays a year later.

By 2009, the streams were ready to merge. The tools existed. The practices existed in scattered pockets. The frustration with the status quo was widespread. What was missing was a name, a community, and a crystallizing event.
