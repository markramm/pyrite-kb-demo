---
id: anderson-economics-of-information-security
title: Why Information Security is Hard — An Economic Perspective
type: source
tags:
- security-economics
- academic-paper
- market-failure
- incentives
- ross-anderson
importance: 7
source_type: academic-paper
date: 2001-01-01
author: Ross Anderson
url: ''
publication: Proceedings of the 17th Annual Computer Security Applications Conference
  (ACSAC)
---

Ross Anderson's 2001 paper "Why Information Security is Hard — An Economic Perspective," presented at the Annual Computer Security Applications Conference, is a foundational document for the field of security economics and one of the key intellectual sources that Schneier drew on and developed in parallel. The paper argues that most information security failures are not technical failures but economic ones: the party responsible for security is often not the party who bears the cost of insecurity, creating systematic market failures in security investment.

## The Core Argument

Anderson's paper identifies several structural reasons why security is systematically underprovided in markets. The most important is misaligned incentives: software vendors face little liability for insecure products because harm falls on users and third parties. Banks and card processors historically had incentives to blame customers for fraud rather than invest in more secure authentication, because the institutional costs of fraud were lower than the costs of better infrastructure. These observations — grounded in economic theory about externalities, moral hazard, and information asymmetry — provided a formal vocabulary for something Schneier had been observing empirically: that security failures were usually deployment and incentive failures, not cryptographic ones.

The paper appeared in the same year as [[secrets-and-lies]], Schneier's own pivot away from purely technical security thinking. The convergence is not coincidental: both Anderson and Schneier were responding to the same observable phenomenon — technically adequate security tools routinely failing in deployment because of organizational and incentive structures. Anderson provided the economic theory; Schneier provided the practitioner's narrative and public reach.

## Relationship to Schneier's [[security-economics]] Concept

Schneier has credited [[ross-anderson]] as a co-founder of the [[security-economics]] field and cited this paper as a foundational text. The paper's influence on [[schneier-on-security-blog]] is visible: many of Schneier's posts analyzing why organizations fail to invest adequately in security echo Anderson's framework about who bears costs and who makes decisions. The same logic underpins Schneier's later arguments in [[click-here-to-kill-everybody]] about IoT security — manufacturers who externalize the security costs of their devices onto users and the internet at large are exhibiting the precise market failure Anderson described in 2001.

## Broader Intellectual Significance

Anderson's paper helped establish security economics as a legitimate academic discipline, with its own conference track (the Workshop on the Economics of Information Security, WEIS, launched 2002) and research community. Schneier's public writing helped broadcast these insights beyond the academic economics-of-security community to policymakers and the general public. The paper thus documents the intellectual tradition from which Schneier's [[security-economics]] framework emerged — essential context for understanding why Schneier frames security as a policy and incentive problem, not merely a technical one.
