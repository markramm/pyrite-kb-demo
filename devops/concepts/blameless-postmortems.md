---
id: blameless-postmortems
title: "Blameless Postmortems"
type: concept
importance: 7
tags:
- learning
- safety-culture
- incidents
- etsy
- just-culture
- organizational-learning
concept_type: pattern
first_appeared: "Etsy engineering culture (John Allspaw, c. 2010-2012); codified in SRE book (2016)"
key_writings:
- site-reliability-engineering-book
- the-devops-handbook
related_concepts:
- site-reliability-engineering
- dev-ops-cooperation
- chaos-engineering
research_status: draft
---

A blameless postmortem is a structured review of a production incident that focuses on systemic causes rather than individual fault. The output is organizational learning — what failed in the system, process, or tooling — not a record of who made a mistake.

## Origins in Safety Science

The concept did not originate in software. Aviation safety, nuclear power operations, and emergency medicine developed analogous practices under the frameworks of "just culture" and human factors engineering. Sidney Dekker's work, particularly "The Field Guide to Human Error" and "Just Culture," provided the theoretical foundation: in complex systems, failures arise from systemic conditions that make errors likely, not from individual negligence or incompetence. Punishing individuals for failures in complex systems destroys learning without improving safety.

[[john-allspaw]], while VP of Engineering at Etsy around 2010-2012, brought this safety science tradition into web operations. He had read the aviation literature and saw direct application to production incidents in high-deployment web engineering. Etsy's postmortem practices became influential — widely referenced and imitated — before appearing in any DevOps book.

## The Logic of Blamelessness

Blame inhibits learning in a specific way: people who fear punishment hide information. An engineer who made a configuration error will minimize, deflect, or stay silent if they expect to be scapegoated. The actual systemic conditions — the confusing deployment interface, the missing validation, the unclear runbook — never surface. The organization repeats the failure.

A blameless environment inverts the incentive. Accurate, detailed accounts of what happened become safe to give. Systems get improved. The engineer who surfaced the failure mechanism is an asset to the investigation rather than a liability to be managed.

This connects directly to Deming's "Drive Out Fear" — Point 8 of the [[demings-journey-to-profound-knowledge|14 Points]]. Deming argued that fear in organizations suppresses quality data. People report what they think is safe to report, not what is actually happening. The same logic applies to incident reports.

## Connection to the Third Way

In Kim's [[three-ways]] framework, blameless postmortems are the primary institutional mechanism for the Third Way — Continual Learning and Experimentation. The Third Way posits that high-performing organizations must generate learning from failure faster than failure can accumulate. Postmortems are the mechanism: structured, recurring, broadly shared processes for converting incidents into improvements.

The [[site-reliability-engineering-book]] codified a specific postmortem template and process: timeline reconstruction, contributing factor analysis, action items with owners. The format mattered less than the cultural commitment. Organizations that practice postmortems consistently outperform those that don't — a finding validated by [[accelerate-book]]'s research on learning culture.

## Egoless Programming Connection

Gerald Weinberg's "egoless programming" concept from "The Psychology of Computer Programming" (1971) is a distant ancestor. Weinberg argued that programmers must not identify personally with their code — code belongs to the team, and criticism of code is not criticism of the person. Blameless postmortems extend this principle to operations: incidents are not personal failures; they are system signals. The organizational equivalent of egoless programming.

## Blameless Culture as a Diagnostic

The practice of blameless postmortems functions as a cultural indicator. Organizations that perform them — and perform them well, not just nominally — have already made a set of commitments: that learning matters more than punishment, that systemic analysis is valued over quick accountability, that engineers can report accurately without career consequences.

Organizations that cannot sustain blameless postmortems reveal something about their culture: fear is present, trust is insufficient, or management prioritizes accountability theater over actual improvement. This makes postmortem practice both a tool and a diagnostic for organizational health.

The [[chaos-engineering]] discipline extends the logic: if blameless postmortems treat accidental failures as learning opportunities, chaos engineering deliberately creates failures to generate learning proactively. The cultural prerequisite is the same.
