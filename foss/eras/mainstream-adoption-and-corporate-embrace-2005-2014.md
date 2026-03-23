---
id: mainstream-adoption-and-corporate-embrace-2005-2014
title: "Mainstream Adoption and Corporate Embrace (2005–2014)"
type: era
tags:
- git
- github
- android
- corporate-embrace
- cloud
- gpl-v3
- linux-foundation
importance: 8
metadata:
  date_range: "2005-2014"
  key_figures: &id001
  - linus-torvalds
  - mitchell-baker
  - jim-zemlin
  key_writings: &id002
  - producing-open-source-software-2005
  - success-of-open-source-weber-2004
  key_concepts: &id003
  - bazaar-model
  - open-core-business-model
  - commons-based-peer-production
  - bdfl-governance
  - release-early-release-often
  - maintainer-sustainability-crisis
  key_events: &id004
  - git-release-2005
  - github-launch-2008
  - gpl-v3-release-2007
  research_status: draft
date_range: "2005-2014"
key_figures: *id001
key_writings: *id002
key_concepts: *id003
key_events: *id004
research_status: draft
---

The decade from 2005 to 2014 saw open source software transition from a developer subculture into the default substrate of commercial computing. Git transformed distributed development; GitHub made contribution accessible to orders of magnitude more developers; Android put Linux into billions of consumer devices; and cloud computing was built almost entirely on FOSS infrastructure. Corporate embrace was total — and with it came the tensions that would define the subsequent era.

## Git and the Transformation of Collaboration (2005)

[[linus-torvalds]] created Git in April 2005 after a licensing dispute ended Linux kernel developers' use of the proprietary BitKeeper system. The [[git-release-2005]] was not merely a new tool but a new model of collaboration: distributed version control meant that anyone could clone a repository, work on it independently, and propose changes back. This decentralized the development workflow in a way that would eventually enable GitHub's pull request model.

Git's adoption extended far beyond the Linux kernel. By the early 2010s, it had become the overwhelmingly dominant version control system across the software industry, displacing Subversion, CVS, and other centralized systems. The [[patch-based-development]] practices of the kernel era gave way to Git-based workflows that are now the universal practice of software development.

## GitHub and the Socialization of Open Source (2008)

[[github-launch-2008]] in April 2008 was a qualitative shift in FOSS participation. GitHub built a social layer on top of Git: pull requests, issue trackers, stars, forks, and contributor graphs made open source contribution legible and social in ways it had never been. Developers who would never have navigated a mailing list or patch submission process could now fork a repository and submit a pull request in minutes.

GitHub lowered the barrier to contribution dramatically, but it also changed the nature of the FOSS community. The new cohort of GitHub-era contributors came to open source through a user-friendly interface rather than through the hacker culture or the free software movement's ethical commitments. This had implications for community culture, maintainer dynamics, and the distribution of labor between core maintainers and occasional contributors — tensions that [[nadia-eghbal]]'s [[roads-and-bridges-2016]] and [[working-in-public-eghbal-2020]] would later analyze.

## Android and Linux in Billions of Devices (2008)

Google's Android operating system, launched in 2008, was built on the Linux kernel. By the mid-2010s, Android was running on billions of smartphones, making Linux the dominant operating system by device count many times over. Android's use of Linux demonstrated the power of copyleft's provisions — Google was required to release the Linux kernel modifications it made under GPL v2 — while also demonstrating its limits: Android's higher-level stack (Java APIs, Google Play Services) was proprietary, producing what critics described as a "copyleft bypass" through architectural choices.

## Corporate Embrace: IBM, Google, Facebook

By the late 2000s, major technology corporations had shifted from viewing open source as a threat to treating it as a strategic asset. IBM invested massively in Linux and the [[linux-foundation]] (formed in 2007 from the merger of OSDL and the Free Standards Group). Google released major infrastructure projects: Go, V8, Android. Facebook released HHVM and React. Amazon built AWS almost entirely on FOSS components. The pattern was consistent: companies that had built proprietary advantages on FOSS infrastructure released projects where collaboration benefited them more than exclusivity would.

This created what critics called "corporate free-riding" — the structural asymmetry between corporations that extracted enormous value from FOSS and communities whose volunteers maintained the infrastructure. The [[maintainer-sustainability-crisis]] was being built during this era, though it would not be widely recognized until after the Heartbleed vulnerability (2014).

## GPL v3 and the Permissive License Shift (2007)

The [[gpl-v3-release-2007]] on June 29, 2007 addressed two problems GPL v2 had not anticipated: "tivoization" (hardware that ran GPL software but used cryptographic locks to prevent users from modifying it) and software patents. The three-year public drafting process was unprecedented in FOSS governance.

GPL v3 was also controversial. The Linux kernel, led by [[linus-torvalds]], explicitly remained on GPL v2. Torvalds was particularly skeptical of GPL v3's patent provisions. The corporate community largely preferred permissive licenses — Apache License 2.0, MIT, BSD — that imposed no copyleft obligations. The decade from 2005 to 2014 saw a measurable shift in the ecosystem: new projects increasingly chose permissive licenses over GPL, partly from corporate preference and partly because the proliferation of cloud computing meant that the GPL's distribution trigger (which applies when distributing software but not when running it as a service) provided weakening protection against proprietary capture.

## Cloud Computing as the GPL Loophole

The growth of cloud computing (AWS launched 2006, Google Cloud, Azure) created a structural challenge to copyleft licensing. The GPL's obligations are triggered by *distribution* — but if a company runs GPL-licensed software as a service rather than distributing it to users, no distribution has occurred and no GPL obligations attach. This "Application Service Provider loophole" or "SaaS loophole" was recognized early but not closed until the Affero GPL (AGPL), which extended copyleft to network use. Corporate resistance to the AGPL was fierce; most major cloud providers' policies prohibit or restrict use of AGPL-licensed components.

## What This Era Established

By 2014, open source had won the infrastructure war: Linux ran the cloud, Git ran version control, and FOSS libraries and frameworks were the default foundation for commercial software development. But this victory carried costs. The [[maintainer-sustainability-crisis]] was building. The [[open-core-business-model]] was under pressure from cloud providers. And the Heartbleed vulnerability — a serious flaw in OpenSSL, maintained by a tiny volunteer team that secured a large fraction of internet traffic — revealed that critical infrastructure was being maintained by people with no resources proportional to the stakes.

The era that followed — [[modern-foss-and-sustainability-crisis-2015-present]] — would be defined by confronting that gap between FOSS's infrastructural centrality and the fragility of its maintenance model.
