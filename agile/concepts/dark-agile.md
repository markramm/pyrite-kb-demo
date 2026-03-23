---
id: dark-agile
title: "Dark Agile"
type: concept
importance: 6
tags:
- anti-pattern
- critique
- dark-scrum
originator: "ron-jeffries"
concept_type: anti-pattern
research_status: draft
---

Dark Agile is the pattern of organizations that adopt Agile ceremonies, roles, and vocabulary without adopting Agile values. The term encompasses several related diagnoses: [[ron-jeffries]]' "Dark Scrum," [[martin-fowler]]'s "Flaccid Scrum," and the broader concept of "doing Agile" versus "being agile." It is the primary failure mode of Agile adoption at scale and the central concern of the [[post-agile-era]] critique.

## What Dark Agile Looks Like

Dark Agile implementations share characteristic patterns:

**Ceremonies without purpose** — Daily Scrums become status reports to the Scrum Master or manager, not coordination among peers. Sprint Reviews become presentations to management, not feedback collection from stakeholders. [[retrospective|Retrospectives]] identify the same problems every Sprint because there is no organizational mechanism to address them.

**Velocity as a weapon** — [[velocity]] is used to pressure teams rather than forecast delivery. "Why is your velocity lower than last sprint?" replaces "What is in the way of the team?" The resulting story point inflation makes planning progressively less useful.

**Sprint as micro-waterfall** — The Sprint boundary replicates the project phase structure: requirements finalized at Sprint Planning, development in the middle, testing at the end. The integration of development and testing that XP's [[test-driven-development]] and [[continuous-integration]] make possible is absent.

**Backlog as requirements dump** — The Product Backlog becomes a backlog in the colloquial sense: a list of things that need to be done, ordered by whoever last touched it, not by value. The Product Owner role is filled by a business analyst who writes stories but has no authority to make trade-off decisions.

**"Agile" as justification for removing protections** — The most damaging dark pattern: Agile's informality and adaptability are invoked to remove documentation, planning, and process safeguards while maintaining or increasing delivery pressure. The result is the worst of both worlds: the overhead of planning is removed, but the accountability and quality checks are removed too.

## Ron Jeffries' "Dark Scrum" Diagnosis

[[ron-jeffries]] — XP co-creator and one of the original advocates for developer-centric Agile — developed the Dark Scrum concept in a series of essays. His argument: Scrum, when adopted by organizations without genuine commitment to its values, gives management new mechanisms to harm developers. The Sprint becomes a two-week deadline. The Daily Scrum becomes micromanagement. The Definition of Done becomes a negotiation the team always loses because they have less organizational power than their stakeholders. Jeffries' diagnosis is that Scrum's lack of prescribed technical practices (unlike [[extreme-programming]]) makes it vulnerable to adoption-without-understanding because there is no floor of technical discipline that must be demonstrated.

## Martin Fowler's "Flaccid Scrum"

[[martin-fowler]] described "Flaccid Scrum" as Scrum adoption without the technical practices: teams running sprints, holding retrospectives, maintaining backlogs — but without [[test-driven-development]], [[continuous-integration]], [[refactoring]], or other practices that make sustained iterative delivery possible. The result is a codebase that degrades sprint by sprint as [[technical-debt]] accumulates, until velocity collapses. Fowler's diagnosis: Scrum without technical practices is unsustainable by design.

## Relationship to the [[agile-industrial-complex]]

Dark Agile is partly an artifact of the [[agile-industrial-complex]]. Certification programs that certify Scrum Masters without requiring practical competence or team experience, and enterprise framework adoptions that prioritize compliance over capability, create a population of "Agile practitioners" who have learned the ceremonies without internalizing the values. The commercial ecosystem has a structural interest in broad adoption; Dark Agile is what broad adoption without genuine commitment produces.
