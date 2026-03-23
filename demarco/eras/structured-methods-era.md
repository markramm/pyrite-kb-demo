---
id: structured-methods-era
title: "Structured Methods Era"
type: era
importance: 7
tags:
- structured-analysis
- structured-design
- software-engineering
- data-flow-diagrams
- measurement
date_range: "1975-1987"
key_writings:
- structured-analysis-and-system-specification
- controlling-software-projects
key_concepts:
- coding-war-games
affiliations:
- yourdon-inc
---

The structured methods era spans roughly 1975 to 1987 — from DeMarco's emergence as a software engineering methodologist through the publication of [[peopleware]], which marked the definitive pivot toward human and organizational concerns. During this period, DeMarco's primary intellectual project was the formalization of software system description: creating rigorous, teachable techniques for modeling information systems before implementation began.

## The structured analysis project

DeMarco's foundational contribution in this era was [[structured-analysis-and-system-specification]] (1978), which systematized the use of data flow diagrams (DFDs), data dictionaries, and process specifications as tools for describing system requirements. The approach addressed a persistent problem in software development: the gap between what clients needed and what developers built, which DeMarco attributed partly to the absence of a shared visual language for describing system behavior.

The structured analysis approach was not purely DeMarco's invention — [[edward-yourdon]] and [[larry-constantine]] had developed parallel structured design methods, and the movement as a whole was a collaborative intellectual enterprise centered on [[yourdon-inc]]. DeMarco's contribution was the requirements side of the equation: while Constantine and Yourdon addressed how to structure software, DeMarco addressed how to discover and specify what the software should do.

## Measurement and control

[[controlling-software-projects]] (1982) extended the structured methods agenda into project management. DeMarco argued that software projects failed partly because they lacked reliable measurement: without objective metrics for progress, scope, and quality, managers could not distinguish between projects on track and projects in crisis. The book proposed a measurement framework — function points, defect rates, productivity metrics — that treated software development as an engineering discipline amenable to quantitative management.

This measurement agenda would later become the target of DeMarco's own [[reflective-era]] self-critique. The 2009 IEEE essay [[software-engineering-an-idea-whose-time-has-come-and-gone]] argued that the emphasis on measurement and control had produced organizations better at managing costs than at producing valuable software — a direct reconsideration of the controlling-software-projects program.

## The Coding War Games: bridge to Peopleware

The empirical work that became [[peopleware]]'s foundation — the [[coding-war-games-study]] — began in approximately 1984, within the structured methods era. The study grew out of DeMarco and [[timothy-lister]]'s consulting and training work, which gave them access to programmers across multiple organizations. The Coding War Games data, showing that environmental and organizational factors dwarfed individual skill in predicting programmer performance, pointed directly away from the structured methods agenda and toward the peopleware argument. The era ends, effectively, when that argument crystallized in the [[peopleware-publication]] of 1987.

## Institutional context

The structured methods era is inseparable from [[yourdon-inc]] as an institution. Yourdon's publishing imprint, consulting network, and training programs provided the distribution channel that gave DeMarco's methods their reach. [[concise-notes-on-software-engineering|*Concise Notes on Software Engineering*]] (1979) is an early DeMarco text from this milieu — a practitioner-oriented survey published by Yourdon Press the year after [[structured-analysis-and-system-specification]]. The move away from Yourdon to [[dorset-house-publishing]] and the [[atlantic-systems-guild]] for Peopleware represents both an intellectual and institutional transition.
