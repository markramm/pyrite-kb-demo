---
id: handbook-of-walkthroughs-inspections-reviews-1990
title: "Handbook of Walkthroughs, Inspections, and Technical Reviews"
type: writing
importance: 7
tags: [code-review, walkthroughs, inspections, software-quality, peer-review]
writing_type: book
date: 1990-01-01
coauthors: [daniel-freedman]
publication: "Dorset House"
key_concepts: [technical-reviews-and-walkthroughs, egoless-programming]
research_status: draft
---

Co-authored with [[daniel-freedman]], this book became the definitive practical guide to [[technical-reviews-and-walkthroughs]] — the systematic peer review of software artifacts. It went through multiple editions, with an earlier version appearing as the [[ethnotechnical-review-handbook-1979]], and became standard reference material in organizations that took code review seriously.

## Core Argument

The book builds on [[egoless-programming]]: reviews work only when participants can separate their personal identity from the code under examination. This is not a pious hope but an organizational design problem. The Freedman-Weinberg approach specifies the structural conditions that make ego-free review possible: distinct roles (author, moderator, reviewers), clear rules about what constitutes in-scope and out-of-scope commentary, separation of defect detection from defect correction, and explicit management of the social dynamics of the review room.

## Three Forms of Review

The book distinguishes walkthroughs, inspections, and technical reviews as distinct practices with different purposes and dynamics. Walkthroughs are author-led — the author presents the work and the audience asks questions. Inspections follow Fagan's structured methodology — formal roles, checklists, metrics, and a defined process. Technical reviews fall between the two — more structured than walkthroughs, less formal than inspections. The taxonomy matters because organizations that treat all reviews as interchangeable tend to do none of them well.

## Significance

The book predates modern code review tools (Gerrit, GitHub pull requests, Phabricator) by decades but established the principles they implement. The standard pull request workflow — submit code, receive line-by-line comments, revise, merge — assumes that developers can give and receive criticism of code without interpersonal breakdown. That assumption was not obvious; Weinberg and Freedman helped build the professional culture in which it became obvious. The "ethnotechnical" framing of the earlier edition reflected Weinberg's anthropological lens — reviews are a cultural practice, and understanding them requires attention to the social dynamics of the review room as much as to the code under examination.
