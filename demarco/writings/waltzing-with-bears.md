---
id: waltzing-with-bears
title: "Waltzing with Bears: Managing Risk on Software Projects"
type: writing
importance: 7
tags:
- book
- risk-management
- project-management
- software-engineering
writing_type: book
date: 2003-01-01
coauthors:
- timothy-lister
publisher: "Dorset House"
key_concepts:
- risk-management-as-risk-embracement
- slack-concept
- organizational-learning-disability
research_status: draft
---

*Waltzing with Bears: Managing Risk on Software Projects* (2003), co-authored by DeMarco and [[timothy-lister]] and published by [[dorset-house-publishing]], is the third major collaboration in the [[peopleware-breakthrough-era]] and [[organizational-dynamics-era]]. Its central argument — that software projects should embrace and explicitly manage risk rather than pretending it doesn't exist — extends the empirical and humanistic orientation of [[peopleware]] into the domain of project planning.

## The risk embracement argument

The book's provocative thesis is captured in its title: organizations that refuse to acknowledge risk do not eliminate it, they merely dance with it blindly. [[risk-management-as-risk-embracement]] is DeMarco and [[timothy-lister]]'s term for the alternative: explicitly identifying, quantifying, and incorporating risk into planning decisions, accepting that uncertainty is inherent in software work rather than a failure of planning discipline.

Conventional project management, they argue, treats risk as something to be mitigated away — buffered against with contingency reserves, managed out of existence through process controls, or simply ignored in favor of optimistic schedules. The result is projects that proceed on assumptions everyone knows to be unrealistic, discovering the risks late when they are most expensive to address.

## The schedule as probability distribution

The book's most technically distinctive contribution is the argument that a project schedule should be expressed as a probability distribution rather than a single date. Every significant uncertainty — a key technology dependency, an unstable requirement, a vendor risk — contributes a range of possible outcomes. Aggregated across a project, these uncertainties produce a distribution of possible completion dates. The single date in a project plan is, at best, the median of this distribution; more often it is the optimistic end.

This reframing has practical consequences: management decisions about risk (which risks to mitigate, which to accept, which to transfer) become decisions about which part of the distribution to shift. The connection to [[slack-concept]] is direct — slack is the buffer capacity that shifts the distribution toward the favorable end.

## Organizational dynamics

Like [[peopleware]] and [[slack]], *Waltzing with Bears* is as much about organizational behavior as about technical methodology. The tendency to present falsely certain schedules is not primarily a failure of estimation skill — it is a response to organizational incentives. Managers who present optimistic schedules are rewarded initially; managers who present realistic (uncertain) schedules face pressure and skepticism. The [[organizational-learning-disability]] that [[peopleware]] describes at the level of project retrospectives appears here at the level of planning culture.

DeMarco and [[timothy-lister]] argue that addressing this requires organizational permission for honest uncertainty — leadership that rewards accurate probability estimates rather than confident single-point predictions. This is, characteristically, a sociological argument about organizational culture rather than a technical argument about estimation methods.

## Relationship to the DeMarco-Lister collaboration

*Waltzing with Bears* is the last major co-authored work before [[adrenaline-junkies-and-template-zombies]] (2008), which expanded the collaboration to the full [[atlantic-systems-guild]]. It represents the mature phase of the DeMarco-[[timothy-lister]] intellectual partnership, applying their established empirical and humanistic approach to a domain — risk — that had previously been dominated by more technical and process-oriented treatments.

The book was received as an important counterweight to the prevailing software project management literature's overconfidence and is cited in both the Agile community (which inherited its skepticism of false certainty) and the risk management literature. It received the [[jolt-award-waltzing-with-bears|2004 Jolt Award]] for best general computing book, and the risk-embracement argument it makes was anticipated by Lister's solo IEEE essay [[lister-risk-management-ieee|"Risk Management Is Project Management for Adults"]] (1997).
