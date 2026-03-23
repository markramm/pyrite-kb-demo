---
id: egoless-programming
title: Egoless Programming
type: concept
tags:
- programming
- psychology
- code-review
- team-dynamics
- software-quality
links:
- target: empower-the-team
  relation: related_to
  note: Egoless programming's trust in collective code ownership prefigures lean empowerment
    of teams
  kb: poppendiecks
importance: 10
first_appeared: psychology-of-computer-programming-1971
source_tradition: social psychology
key_writings:
- psychology-of-computer-programming-1971
related_concepts:
- technical-reviews-and-walkthroughs
- programming-as-human-activity
- congruent-behavior
- moi-model
research_status: draft
---

Egoless programming is [[gerald-weinberg]]'s proposal, first articulated in [[psychology-of-computer-programming-1971]], that software quality improves when programmers learn to separate their personal identity from their code. The idea is simple to state and difficult to practice: code is an artifact, not an extension of the self, and treating it as such opens the door to honest, productive review.

## The Core Idea

Weinberg observed that programmers in the early 1970s — like craftspeople in any discipline — tended to identify deeply with their work. A criticism of the code felt like a criticism of the person. This conflation produced a range of counterproductive behaviors: defensiveness during reviews, reluctance to ask for help, hoarding of code, and an unwillingness to admit errors. Egoless programming was Weinberg's term for the discipline of detaching ego from code so that bugs could be found and fixed without the friction of wounded pride.

Weinberg articulated ten "commandments" of egoless programming, including: understand and accept that you will make mistakes; you are not your code; no matter how much you know, someone else will always know more; don't rewrite code without consultation; treat people who know less than you with respect; the only constant in the world is change; the only true authority stems from knowledge; fight for what you believe, but gracefully accept defeat; don't be the coder in the corner; critique code instead of people.

## Common Misreading

Egoless programming is frequently misread as "have no ego" or "suppress your personality." This is not what Weinberg meant. He was not advocating for programmers to become passive or self-effacing. He was advocating for a specific and bounded form of non-attachment: keep your sense of self, but do not locate it in the particular lines of code you wrote this week. The ego remains; it just doesn't live in the diff.

This distinction matters practically. A programmer with no ego might accept any criticism without evaluation. A programmer practicing egoless programming evaluates criticism on its technical merits, accepts valid criticism without defensiveness, and pushes back on invalid criticism without feeling personally attacked.

## Lineage and Influence

Egoless programming is arguably the most influential idea Weinberg ever articulated, even though it is rarely attributed to him by name in contemporary practice.

The direct lineage runs through [[technical-reviews-and-walkthroughs]], codeveloped with [[daniel-freedman]], which formalized the structural conditions under which egoless review could happen. Structured walkthroughs required, among other things, that the author of code not act as moderator of the review — a procedural embodiment of egoless principles.

Kent Beck's Extreme Programming, described in the late 1990s, reintroduced several egoless programming principles under new names. Collective code ownership — the XP practice of treating all code as belonging to the team rather than any individual — is a direct institutional expression of the egoless insight. Pair programming creates continuous, low-stakes peer review. Beck cited Weinberg's influence.

The open source movement operationalized egoless programming at scale. The norm of public patch submission, code review on mailing lists, and maintainer rejection of patches — without the author treating rejection as personal insult — required exactly the ego-code separation Weinberg described. Linus Torvalds famously violated this norm in his personal communications while institutionalizing it structurally in the Linux development process.

Modern code review tools (Gerrit, GitHub pull requests, Phabricator) are the industrial infrastructure for egoless programming. The standard pull request workflow — submit code, receive comments, revise, merge — assumes that authors can receive line-by-line criticism of their work without interpersonal breakdown. This assumption was not obvious in 1971; Weinberg helped make it obvious.

## Connection to Weinberg's Broader Project

Egoless programming is the entry point into [[programming-as-human-activity]], Weinberg's meta-thesis. If programming were a purely technical activity, ego would be irrelevant — computers don't care about programmers' feelings. The fact that ego attachment to code is a major source of quality problems is evidence that programming is a human activity, shaped by social dynamics, self-image, and group psychology. Egoless programming is thus both a practical heuristic and an argument for Weinberg's entire intellectual project.

The concept also connects to [[congruent-behavior]] from Weinberg's later work with Virginia Satir's model. The defensive programmer who cannot hear criticism of their code is exhibiting incongruent behavior — specifically the blaming stance, in which self and context are attended to but others are discounted. Egoless programming creates the conditions for congruence.
