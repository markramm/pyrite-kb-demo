---
id: inrupt
title: "Inrupt"
type: organization
importance: 6
tags:
- decentralization
- data-ownership
- solid
- web
- security-architecture
org_type: company
founded: "2017"
location: "Boston, Massachusetts"
url: "https://www.inrupt.com"
---

Inrupt, Inc. is the company commercializing the Solid standard, a technical framework for decentralized, user-controlled data storage on the web. Founded by [[tim-berners-lee]] and John Bruce in 2017, Inrupt is building the enterprise and consumer infrastructure to make Solid deployable at scale. Schneier joined the company as Chief of Security Architecture, a role that places him at the intersection of web-scale architecture and the data-ownership problem he diagnosed in [[data-and-goliath]].

## The Solid Standard

Solid (Social Linked Data) proposes that users store their personal data in "pods" — Solid-compatible servers they control — and grant applications permission to read and write specific data rather than surrendering data to each application's silo. The architecture is designed to separate data from applications: you could switch social networks, productivity tools, or health apps while retaining your data and history. This directly addresses the lock-in and concentration dynamics that make surveillance capitalism structurally stable.

The security design challenges for Solid are substantial. A decentralized data architecture must solve identity (who is accessing the pod?), authentication (how do you verify identity across a distributed system?), authorization (which applications can access which data?), and auditability (how do you know what has been accessed?) — all at web scale and without the centralized control that makes these problems tractable for platform companies. Schneier's role is to ensure the security architecture is sound and that the system's trust model is coherent, drawing on the [[trust-framework]] analysis he developed across books from [[liars-and-outliers]] through [[a-hackers-mind]].

## Connection to Schneier's Security Economics Analysis

[[data-and-goliath]] argued that the surveillance economy emerged from a structural asymmetry: data collection is cheap, its value is concentrated in the hands of collectors, and the people whose data is collected bear diffuse harms without effective recourse. Inrupt's bet is that this asymmetry can be addressed by technical architecture — if users control their data in portable pods, the platform lock-in that enables surveillance capitalism weakens, and some of the value flows back to data subjects.

Schneier's [[security-economics]] framework would predict that this technical solution only works if the incentive structure changes: companies must find it in their interest to build Solid-compatible systems rather than proprietary silos. Inrupt's enterprise strategy — selling Solid infrastructure to large institutions (banks, healthcare systems, governments) that have regulatory and reputational incentives to give users data control — is an attempt to create those incentives. Whether this market strategy can succeed against the network effects of incumbent platforms is the central question for Inrupt's future, and it is precisely the kind of incentive-structure problem that Schneier's security economics framework is designed to analyze.
