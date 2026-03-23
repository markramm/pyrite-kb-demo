---
id: who-does-that-server-really-serve
title: Who Does That Server Really Serve?
type: writing
tags:
- saas
- cloud-computing
- software-freedom
- essay
- network-services
importance: 7
writing_type: essay
date: 2010-03-01
coauthors: []
publication: Boston Review / GNU Project
url: https://www.gnu.org/philosophy/who-does-that-server-really-serve.html
key_concepts:
- saas-loophole
- four-freedoms
- free-software-definition
- digital-restrictions-management
research_status: draft
---

"Who Does That Server Really Serve?" (originally published in Boston Review, 2010) is [[stallman]]'s analysis of software-as-a-service (SaaS) and cloud computing as a challenge to software freedom. The essay extends the [[four-freedoms]] framework to networked services, arguing that when users run programs on someone else's server rather than their own computer, they lose the same freedoms that proprietary software denies — even if the server software is licensed under the GPL.

The core argument is about the [[saas-loophole]]: the GPL's copyleft obligations are triggered by distribution of software, not by running software as a service. A company can take GPL-licensed software, improve it extensively, and run it as a web service that millions of people use, without ever releasing the improvements. Users who depend on such a service have no ability to study what it does, no ability to modify it, and no ability to run their own version. The [[agpl]] partially addresses this, but only for software specifically licensed under it.

The essay identifies a more fundamental problem than licensing: even if the server software were AGPL-licensed and all modifications were available, the user is still dependent on the service provider's hardware, infrastructure, and continued willingness to operate the service. The service as computing — as the locus of the user's actual work — remains outside the user's control.

[[stallman]] distinguishes between two cases: services that perform functions on behalf of users (a translation service, a search engine) and services that store or process users' own data (a word processor in the cloud, email, social networking). The first category is relatively benign: there is no particular reason you need to run your own translation service. The second category is the problem: when your documents, communications, and data are processed by someone else's server under terms you cannot inspect or modify, you have lost something analogous to what proprietary software takes from you.

The essay connects to the broader trajectory of the [[gplv3-and-later-career-2006-present]] era, when the dominant threats to software freedom had shifted from proprietary desktop software to cloud services, mobile platforms locked to vendor-controlled app stores, and hardware with locked boot chains. [[stallman]]'s response across this era is consistent: the [[four-freedoms]] must be extended to cover these new forms of computing if they are to remain meaningful, not treated as exceptions because the technical form is different.
