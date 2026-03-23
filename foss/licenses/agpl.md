---
id: agpl
title: "GNU Affero General Public License"
type: license
importance: 6
license_type: copyleft-strong
author: "Free Software Foundation"
date: 2007-11-19
spdx_id: "AGPL-3.0-only"
key_provisions:
- "All provisions of GPL v3"
- "Section 13: network use triggers source disclosure requirement"
- "If users interact with the software over a network, they must be offered the source code"
- "Closes the 'SaaS loophole' in GPL v2 and v3"
related_licenses:
- gpl-v3
- gpl-v2
- sspl-bsl
tags:
- copyleft-strong
- fsf
- saas-loophole
- network-copyleft
- cloud
research_status: draft
---

The GNU Affero General Public License version 3, published by the [[free-software-foundation]] on November 19, 2007, shortly after [[gpl-v3]] in June 2007. The AGPL closes the "SaaS loophole" — the gap in [[gpl-v2]] and [[gpl-v3]] that allows software-as-a-service providers to use and modify GPL software without distributing their modifications, because they never "distribute" the software in the traditional sense.

## The SaaS Loophole

The GPL licenses — both [[gpl-v2]] and [[gpl-v3]] — require source disclosure only when you *distribute* the software. If you run GPL software on a server and allow users to interact with it over a network, you are not distributing the software to those users: you are providing a service. This interpretation means that a company could take GPL-licensed server software, make modifications, and run it as a service without ever releasing those modifications.

This was a theoretical concern in 2007; it became concretely significant as cloud computing matured. A hosting provider can run a modified version of GPL-licensed database software for thousands of customers without releasing a single line of source code. From the free software perspective, this denies those customers [[four-freedoms]] to study and modify the software they depend on.

The Affero company (now defunct) identified this gap in 2002 and created an early version of the Affero GPL (AGPLv1) to address it. The FSF incorporated the fix into AGPLv3, making it an official GNU license.

## Section 13

AGPL's key addition to GPL v3 is Section 13: if you run a modified version of AGPL software on a server and allow users to interact with it over a network, you must offer those users access to the corresponding source code. The offer must be made prominently, typically via a link in the application's interface.

This is a genuine extension of copyleft to the network context, not just a restatement of GPL's distribution requirement.

## Adoption

The AGPL has been adopted by projects where the SaaS loophole is particularly significant: server-side software with clear commercial value. MongoDB used AGPL before switching to [[sspl-bsl]] in 2018. Mastodon, the federated social network, uses AGPL. Many SaaS infrastructure tools use AGPL specifically because they want cloud providers to either release modifications or negotiate a commercial license.

The "AGPL as business model" pattern became explicit in the [[modern-foss-and-sustainability-crisis-2015-present]] era: companies release server software under AGPL, which prevents cloud providers from offering it as a service without releasing modifications; companies then offer a commercial license to cloud providers and others who cannot accept AGPL terms. This dual-licensing model sits at the boundary of [[open-core-business-model]].

The AGPL is incompatible with some other licenses, and several organizations (including Google) have internal policies against using AGPL-licensed software, citing uncertainty about what "network interaction" requires and the difficulty of auditing compliance across large codebases. This corporate resistance to AGPL led some projects to seek even stronger protections — which the [[sspl-bsl]] attempted to provide, at the cost of departing from OSI-approved open source.
