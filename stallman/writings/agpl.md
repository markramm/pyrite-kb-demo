---
id: agpl
title: "GNU Affero General Public License"
type: writing
importance: 7
tags:
- license
- copyleft
- agpl
- free-software
- legal
- saas
- network-services
writing_type: license-text
date: 2007-11-19
coauthors: []
publication: "Free Software Foundation"
url: "https://www.gnu.org/licenses/agpl-3.0.html"
key_concepts:
- copyleft
- gpl-copyleft-mechanism
- saas-loophole
- free-software-definition
research_status: draft
---

The GNU Affero General Public License (AGPL), version 3, released November 19, 2007, closes the [[saas-loophole]] — the gap in [[gpl-v2]] and [[gpl-v3]] that allows companies to run modified GPL software as a network service without releasing the modifications to users.

The loophole arises from the GPL's trigger: copyleft obligations attach when software is "distributed." Running software on a server and letting users interact with it over a network is not "distribution" in the GPL's legal sense — no copy of the software is transferred to the user. A company can therefore take GPL-licensed server software, make extensive proprietary improvements, and run it as a service indefinitely without ever releasing those improvements. This became an increasingly significant issue as web services supplanted desktop software during the [[gplv3-and-later-career-2006-present]] era.

The AGPL addresses this with section 13: if modified AGPL software is used to provide a network service, users interacting with the service must be provided a way to obtain the source code of the modified version they are interacting with. The trigger shifts from "distribution" to "use to provide a service to remote users."

The Affero General Public License existed before [[stallman]] and [[eben-moglen]] formalized it into the GNU license family. The Affero organization had released version 1 in 2002 under a similar provision as an amendment to GPL v2. The FSF's AGPL v3 of 2007 replaced this with a fully integrated license compatible with [[gpl-v3]].

The AGPL has been adopted by a notable range of database, infrastructure, and application projects that want to ensure service providers cannot "embrace and extend" their code without contributing back: MongoDB (before its controversial SSPL shift), Nextcloud, Mastodon, and others. Its practical impact is debated: many large cloud providers simply avoid AGPL software entirely rather than comply, which is itself a form of the license working as designed — it makes free-riding by cloud providers more costly. [[stallman]] endorses the AGPL as the appropriate license whenever the GPL's freedoms need to extend to users of network services, not just recipients of distributed software. The essay [[who-does-that-server-really-serve]] expresses the philosophical case for this extension.
