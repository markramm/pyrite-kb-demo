---
id: technical-reviews-and-walkthroughs
title: Technical Reviews and Walkthroughs
type: concept
tags:
- code-review
- software-quality
- peer-review
- inspection
- process
links:
- target: build-integrity-in
  relation: related_to
  note: Weinberg's structured reviews are a practice for building integrity into software
    through collaborative quality
  kb: poppendiecks
importance: 8
first_appeared: psychology-of-computer-programming-1971
source_tradition: inspection methods (Fagan)
key_writings:
- handbook-of-walkthroughs-inspections-reviews-1990
- psychology-of-computer-programming-1971
related_concepts:
- egoless-programming
- programming-as-human-activity
- quality-software-management-framework
- cultural-patterns-of-software-organizations
research_status: draft
---

Technical reviews and walkthroughs are systematic, structured forms of peer review applied to software artifacts — code, design documents, requirements specifications, test plans. [[gerald-weinberg]] was among the first to write seriously about peer review of software, beginning with [[psychology-of-computer-programming-1971]], and the practice was most fully codified in [[handbook-of-walkthroughs-inspections-reviews-1990]], written with [[daniel-freedman]].

## Lineage

The intellectual lineage of structured software review has two main sources that Weinberg brought together:

**Egoless programming.** In [[psychology-of-computer-programming-1971]], Weinberg described [[egoless-programming]] as the psychological precondition for effective peer review. You cannot review code well — as author or reviewer — if you are defending your ego rather than the quality of the software. Structured reviews needed to embody this principle procedurally, not just exhort programmers to have the right attitude.

**Fagan inspections.** Michael Fagan at IBM (where Weinberg had worked) developed the formal inspection method in the 1970s — a highly structured process with defined roles (moderator, author, reader, inspector), defined phases (planning, overview, preparation, inspection meeting, rework, follow-up), and quantitative defect data collection. Fagan's inspections were rigorous and data-driven but also expensive and administratively intensive.

Weinberg and Freedman's contribution was to describe a range of review methods from lightweight walkthroughs through full formal inspections, with practical guidance on when each is appropriate — not a one-size-fits-all prescription but a menu of tools.

## Key Structural Principles

The Handbook articulated principles that have been absorbed into modern code review practice without attribution:

**Separate author and moderator.** The person who wrote the code should not run the review of it. This is the procedural expression of egoless programming: giving the author control of the review process creates structural conditions for ego defense.

**Review the artifact, not the author.** Comments are about the code, not the person. This norm, stated explicitly in the Handbook, is now a standard of professional code review culture.

**Use checklists.** Different types of artifacts have different types of common defects. Checklists direct reviewer attention to known problem areas rather than relying on each reviewer to reinvent what to look for.

**Small batches.** Reviews are most effective on manageable chunks. Long sessions reviewing large amounts of code produce diminishing returns. This prefigures the modern continuous integration norm of small, frequent pull requests.

**Collect data.** What types of defects are found? At what rates? By which methods? Data from reviews can guide process improvement. This connects to [[quality-software-management-framework]]'s emphasis on first-order measurement.

## Relationship to Modern Code Review

Contemporary code review tools — Gerrit, GitHub pull requests, GitLab merge requests, Phabricator — implement the social and procedural infrastructure that Weinberg and Freedman described two decades before those tools existed. The pull request workflow: author submits, reviewers comment, author revises, reviewer approves, maintainer merges — is a lightweight walkthrough implemented in software.

The norms that make these workflows function (separate the code from the person, comment on the artifact, maintain professional tone, accept valid feedback gracefully) are the egoless programming principles that Weinberg articulated in 1971. They are now so embedded in software development culture that their origin is invisible — which is evidence of successful diffusion, not evidence that they were obvious.

## Within the QSM Framework

In [[quality-software-management-framework]] terms, technical reviews are a feedback mechanism — a way for the organization to learn about the quality of its artifacts before they reach production. Pattern 0 organizations have no such mechanism. Pattern 2 organizations may have reviews as a required process step but lack the [[congruent-behavior]] to make them honest and effective. Pattern 3 and 4 organizations have reviews that genuinely inform their understanding of software quality and drive process improvement.

This means that the quality of a review process is not just a matter of having the right procedures — it depends on the organization's cultural pattern and the congruence of its participants. Weinberg was always insistent on this: process alone doesn't produce quality; process combined with appropriate human dynamics does.
