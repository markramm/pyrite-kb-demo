---
id: bug-triage-and-tracking
title: "Bug Triage and Tracking"
type: practice
tags:
- bugzilla
- issue-tracking
- triage
- quality-assurance
- contributor-onboarding
importance: 4
metadata:
  practice_type: development
  originated_in: "Mozilla project (Bugzilla)"
  related_practices: &id001
  - code-review-in-foss
  - mentorship-programs-gsoc
  - release-management
  status: active
  research_status: draft
practice_type: development
originated_in: "Mozilla project (Bugzilla)"
related_practices: *id001
status: active
research_status: draft
---

Systematic bug management became a distinctive FOSS practice through the need to coordinate distributed volunteer contributors who lack the shared physical context and implicit prioritization of a co-located team. The [[mozilla-foundation]]'s Bugzilla (1998) was the first major web-based bug tracker designed for open source development. Bugzilla emerged from Netscape's internal bug tracking system (also called Bugzilla) and was open-sourced as part of the broader [[netscape-source-release-1998|Mozilla project]]. It introduced features that became standard across all subsequent bug trackers: severity and priority classification, component assignment, keyword tagging, dependency tracking between bugs, customizable workflows, and — critically — public visibility of all bug reports and their full discussion history.

The Bugzilla model established conventions that persist across the FOSS ecosystem even as the specific tooling has evolved. Bug triage — the process of reviewing incoming reports, confirming reproducibility, assigning severity and priority, and routing to the appropriate component maintainer — became a recognized role in FOSS projects, often performed by contributors who were not themselves developers. This was significant: triage created a contribution path for people with domain knowledge and organizational skill but without coding ability, broadening the definition of "contributor" beyond patch submission. The Mozilla project's triage process, with its "bug days" and structured triage meetings, influenced how other large FOSS projects managed their incoming bug flow.

The tooling evolution followed a trajectory from specialized FOSS tools toward integrated platforms. Bugzilla dominated the 2000s but was supplemented and eventually challenged by alternatives: Trac (which integrated bug tracking with wiki and version control), Launchpad (Canonical's platform for Ubuntu and related projects), and Redmine. The [[github-launch-2008|GitHub]] Issues system, introduced as part of GitHub's repository hosting, represented a philosophical shift: rather than a standalone, feature-rich bug tracker, GitHub Issues offered a lightweight, integrated issue system that traded Bugzilla's extensive metadata and workflow customization for simplicity and tight coupling with pull requests. This tradeoff — power versus accessibility — mirrors the broader pattern seen in [[code-review-in-foss]] and [[patch-based-development]].

The "good first issue" label convention, which emerged on [[github-platform]] in the mid-2010s (approximate), represents an important evolution in how bug tracking intersects with community building. By tagging issues that are suitable for newcomers — well-scoped, well-documented, not requiring deep codebase knowledge — projects create an explicit onboarding pathway that connects bug triage to [[mentorship-programs-gsoc|contributor mentorship]]. Issue templates, labels, milestones, and project boards have become standard project management tools across FOSS, extending bug tracking into broader project coordination. The irony is that commercial project management tools like Jira — which are not themselves FOSS — are now widely used by FOSS projects and were significantly influenced by the conventions that Bugzilla established.
