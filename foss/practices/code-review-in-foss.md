---
id: code-review-in-foss
title: "Code Review in FOSS"
type: practice
tags:
- code-review
- quality
- mailing-list
- pull-request
- governance
metadata:
  practice_type: quality
  originated_in: "Linux kernel, Apache"
  related_practices: &id001
  - patch-based-development
  - release-management
  status: active
  research_status: draft
practice_type: quality
originated_in: "Linux kernel, Apache"
related_practices: *id001
status: active
research_status: draft
---

Code review in FOSS predates the formal code review practices of commercial software engineering. Where commercial code review emerged from structured inspection methods (Fagan inspections, 1970s) and was typically a mandated process within an organization, FOSS code review emerged organically from the mailing list collaboration model: when patches are posted publicly, any subscriber can read, critique, and respond. The result is a public, archived, searchable review record — a transparency that commercial code review rarely achieves. The Linux kernel and the [[apache-software-foundation]]'s projects were early exemplars of this model, where rigorous mailing list review became the primary quality gate.

The mailing list review model had distinctive strengths. Reviews were deep and technical — kernel mailing list reviewers routinely analyzed patches for correctness, style, performance implications, and architectural fit. The public nature of review created reputational incentives: reviewers built standing through the quality of their critiques, and contributors learned by observing reviews of others' patches. [[linus-torvalds]]'s notoriously direct review style — sometimes harsh to the point of hostility — was extreme but representative of a culture that prioritized technical rigor over social comfort. This culture contributed to the observation codified as [[linuss-law]]: "given enough eyeballs, all bugs are shallow." The empirical validity of that claim is debatable, but the underlying mechanism — many independent reviewers examining publicly posted code — is real and distinctive to FOSS.

The evolution from mailing list review to web-based review tools followed the broader trajectory of [[patch-based-development]]. Gerrit (developed by Google for Android, later adopted by many projects including the Linux kernel's Gerrit instance for some subsystems), Phabricator (developed at Facebook, used by projects including PHP and Wikimedia), and ReviewBoard offered structured review workflows with inline commenting, approval gates, and integration with continuous integration systems. These tools preserved the substance of mailing list review — public, detailed, technical — while adding structure and discoverability.

The pull request model introduced by [[github-launch-2008|GitHub]] made code review dramatically more accessible but arguably more superficial. PR review lowers the barrier to participation: anyone with a GitHub account can comment on a pull request, and the diff view with inline comments is more approachable than reading patches in an email thread. However, the PR model also enables checkbox-style review — a quick "LGTM" (looks good to me) approval that satisfies the process requirement without deep engagement. The cultural shift from mailing list review (where non-response is the default and approval requires active engagement) to PR review (where approval is a button click) has implications for code quality that the FOSS community has not fully reckoned with. [[karl-fogel]]'s [[producing-open-source-software-2005]] discussed review practices extensively, but the landscape has shifted substantially since its publication.
