---
id: release-early-release-often
title: "Release Early, Release Often"
type: concept
importance: 6
concept_type: development-model
first_appeared: "cathedral-and-the-bazaar-1997"
key_writings:
- cathedral-and-the-bazaar-1997
- producing-open-source-software-2005
related_concepts:
- bazaar-model
- linuss-law
- bdfl-governance
- commons-based-peer-production
tags:
- development-model
- feedback-loops
- bazaar
- continuous-delivery
- agile
- release-management
research_status: draft
---

"Release early, release often" is one of the core principles of the [[bazaar-model]], articulated by [[eric-raymond]] in [[cathedral-and-the-bazaar-1997]] as a key lesson from the Linux kernel's development process. The principle has two parts, each inverting a cathedral-model assumption. Release early: do not wait until the design is polished and the implementation is stable before showing it to users; put working code in front of people while the architecture is still malleable enough to respond to feedback. Release often: maintain a rapid cadence of releases to keep the feedback loop short, sustain contributor engagement, and make each increment small enough that regressions are easy to identify and fix. [[linus-torvalds]]'s management of the Linux kernel — releasing new versions every few weeks in the early 1990s, treating users as co-developers whose bug reports were a primary input to the development process — was Raymond's central example.

The principle's logic connects directly to [[linuss-law]]: "given enough eyeballs, all bugs are shallow." Frequent releases maximize the number of eyes on the code at any given time and minimize the distance between when a bug is introduced and when it is observed. If you release once a year, a bug introduced in month two sits undetected for ten months; if you release every two weeks, the same bug is caught within a release cycle. But the principle goes beyond bug-finding. Early release means the project's design evolves in response to actual use rather than anticipated use. The cathedral model assumes that architects can predict user needs and design accordingly; the bazaar model assumes they cannot and substitutes rapid iteration for upfront planning. This is the same epistemological move that would later appear in Agile software development's preference for "working software over comprehensive documentation" and "responding to change over following a plan."

The influence of release-early-release-often on broader software development practice is difficult to overstate. Continuous integration — the practice of merging developer changes into a shared mainline frequently, with automated testing on each merge — is a formalization of the "release often" principle for internal development. Continuous delivery extends it to production deployment: every change that passes tests is a candidate for release. The Agile Manifesto (2001) enshrined short iterations and frequent delivery as core principles, and while the Agile movement drew on many sources, the FOSS demonstration that rapid release cycles worked at scale — the Linux kernel being the most visible proof — provided concrete evidence that the approach was viable for large, complex software. [[git-release-2005]] itself enabled more fluid release practices by making branching and merging cheap, removing a technical bottleneck that had constrained release frequency in centralized version control systems.

Modern FOSS has formalized the principle in several distinct release strategies. Rolling releases (Arch Linux, Gentoo) take the idea to its logical extreme: there are no discrete version numbers, only a continuously updated stream of packages. Time-based release trains (Ubuntu's six-month cycle, GNOME's six-month cycle, the Linux kernel's current approximately eight-week cycle) regularize the cadence, decoupling the release schedule from feature completion — a release ships whatever is ready on the scheduled date, rather than waiting for a planned feature set. Nightly and beta builds (Firefox, Rust, many others) provide early-adopter feedback channels separate from stable releases. Semantic versioning (semver) — the convention of MAJOR.MINOR.PATCH version numbers — added a communication layer: the version number itself signals whether a release contains breaking changes, new features, or bug fixes, helping users decide when to upgrade.

The principle has limits that Raymond's original articulation did not fully address. Releasing too early can erode user trust if the software is genuinely broken; releasing too often can overwhelm maintainers and downstream packagers with update fatigue. The left-pad incident (2016) — where a single developer's removal of a trivial npm package broke thousands of builds — illustrated a different risk: in ecosystems with very frequent releases and deep dependency chains, the rapid release cadence propagates instability as well as fixes. The [[maintainer-sustainability-crisis]] adds another dimension: release-early-release-often assumes a community of contributors who respond to releases with feedback and patches, but in the [[modern-foss-and-sustainability-crisis-2015-present]] era, many projects have large user bases and tiny contributor bases, meaning frequent releases increase the maintainer's workload without proportionally increasing the feedback that makes the practice valuable.
