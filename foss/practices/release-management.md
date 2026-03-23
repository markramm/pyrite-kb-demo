---
id: release-management
title: "Release Management"
type: practice
tags:
- releases
- stability
- lts
- time-based
- rolling-release
- distribution
metadata:
  practice_type: release-management
  originated_in: "GNU Project, Linux kernel, Debian"
  related_practices: &id001
  - patch-based-development
  - code-review-in-foss
  - bug-triage-and-tracking
  status: active
  research_status: draft
practice_type: release-management
originated_in: "GNU Project, Linux kernel, Debian"
related_practices: *id001
status: active
research_status: draft
---

Release management in FOSS addresses a tension that does not exist in the same way in proprietary software: how does a project with no central product management, no marketing calendar, and contributors who work on their own schedules decide when to ship? The answer varies dramatically across projects and has evolved significantly over the movement's history. The major models — time-based releases, feature-based releases, rolling releases, and Long Term Support (LTS) — each represent a different resolution of the tradeoff between stability and freshness, and between contributor autonomy and user predictability.

The Linux kernel's release history illustrates the evolution. Through the 2.6 series (pre-2004, approximate), the kernel used a feature-based release model: a new version shipped when the planned features were ready, with odd-numbered minor versions (2.1, 2.3, 2.5) serving as unstable development branches and even-numbered versions (2.0, 2.2, 2.4) as stable releases. This model created long, unpredictable release cycles — the 2.5 development series lasted over two years. [[linus-torvalds]] shifted to a time-based model around 2004: new kernel versions release approximately every 10 weeks (currently approximately 9-10 weeks), regardless of which features are ready. Features that miss the merge window wait for the next cycle. This shift was a governance decision as much as a technical one — it reduced the pressure to rush features into a release and made the development rhythm predictable for both contributors and downstream consumers like distributions.

The [[debian-project]]'s stable/testing/unstable model created a layered approach that influenced many derivative distributions. Packages enter unstable (Sid), migrate to testing after a quarantine period without release-critical bugs, and testing eventually freezes and becomes the next stable release. Stable releases receive only security updates and critical fixes, providing the reliability that enterprise and server users require. Ubuntu, Debian's most prominent derivative, adopted a time-based model with releases every six months and LTS releases every two years, maintained for five years. This regularized cadence gave downstream users — particularly enterprise users — predictability that Debian's variable freeze-to-release cycle did not always provide.

Rolling release distributions — Arch Linux, Gentoo, and others — reject the release model entirely: packages update continuously, there are no version numbers, and users always run the latest available software. This model suits users who want current software and are willing to accept occasional breakage, but it creates challenges for reproducibility, support, and the kind of stability guarantees that the [[linux-foundation]] and enterprise consumers require. The existence of all these models simultaneously in the FOSS ecosystem — from Debian stable's multi-year cycles to Arch's daily updates — reflects the movement's pluralism: different communities optimize for different values, and the [[release-early-release-often]] philosophy articulated by [[eric-raymond]] in [[cathedral-and-the-bazaar-1997]] is only one position in a broader landscape of release strategies.
