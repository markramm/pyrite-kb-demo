---
id: controlling-software-projects
title: "Controlling Software Projects: Management, Measurement, and Estimates"
type: writing
importance: 7
tags:
- book
- software-measurement
- estimation
- project-management
- metrics
writing_type: book
date: 1982-01-01
publisher: "Yourdon Press"
key_concepts:
- coding-war-games
- organizational-learning-disability
research_status: draft
---

*Controlling Software Projects: Management, Measurement, and Estimates* (1982), a DeMarco solo work published through [[yourdon-inc]], is a systematic treatment of software measurement and estimation that sits between his [[structured-methods-era]] methodology work and the humanistic arguments of [[peopleware]]. The book established DeMarco as one of the first serious thinkers about software metrics and project control, and its empirical orientation directly prepared the ground for the [[coding-war-games-study]] that would anchor *Peopleware* five years later.

## The measurement argument

The core claim of *Controlling Software Projects* is that software projects cannot be managed in any serious sense without measurement, and that the metrics actually in use in the software industry in the early 1980s were either absent or systematically misleading. Lines of code, then the dominant measure of programmer productivity, were both unreliable (different languages produce different LOC counts for the same functionality) and perverse (optimizing for LOC incentivizes verbosity, not efficiency).

DeMarco proposed function points — a measure of software functionality derived from requirements rather than implementation — as a more meaningful basis for estimation and control. He developed methods for estimating function point counts from requirements specifications, for translating function point estimates into schedule and effort projections, and for calibrating these estimates using historical project data.

## The control model

The book's project control model was built around the feedback loop: measure the current state of the project, compare it to the plan, identify variance, and adjust. This sounds obvious but was genuinely novel as a systematic proposition for software projects. DeMarco argued that most software project management was effectively open-loop — managers pushed toward deadlines without reliable information about actual progress — and that the result was the endemic schedule overruns and cost blowouts that characterized the industry.

The measurement-based control approach required organizations to collect and retain historical project data, calibrate estimation models against their own track records, and build institutional knowledge about their own performance. This anticipates the [[organizational-learning-disability]] argument of [[peopleware]] — an organization that doesn't measure cannot learn from its failures.

## Relationship to the Peopleware arc

*Controlling Software Projects* represents the most technically oriented point in DeMarco's intellectual arc. It treats the software management problem as primarily quantitative and methodological: if you have good data and good estimation models, you can control projects. [[peopleware]] argues that this framing, while not wrong, misses the deeper problem — that the variance in project outcomes is more strongly predicted by organizational and sociological factors than by planning and estimation quality. The empirical work that would produce [[coding-war-games]] data was in part a continuation of the measurement tradition of this book, extended from process metrics to environmental and organizational variables.

The two books together establish the empirical core of DeMarco's work: he is, consistently, a practitioner who wants data and distrusts management theory that is not grounded in measurement. This orientation distinguishes him from more purely humanistic management writers and makes the [[peopleware-thesis]] more compelling — the sociological argument is backed by numbers.
