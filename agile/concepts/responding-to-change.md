---
id: responding-to-change
title: "Responding to Change"
type: concept
importance: 7
tags:
- manifesto
- values
- adaptability
originator: "agile-manifesto-signatories"
concept_type: principle
research_status: draft
---

"Responding to change over following a plan" is value 4 of the [[agile-manifesto-four-values]] and the adaptive core of the movement. It encodes a specific claim about the nature of software development: that requirements are discovered through the process of building, not specified at the outset. Planning is necessary, but plans become progressively less accurate as a project extends into the future, and organizations that treat plans as commitments rather than hypotheses pay a compounding cost in misalignment.

## The Planning Problem in Software

The value targets a specific organizational pattern: treating a project plan approved at the start as a contract that defines what success means at the end. In this model, changes to scope are deviations requiring escalation, re-planning, and renegotiation. The organizational incentive is to suppress change-reporting, which means that misalignment between the plan and reality accumulates invisibly until it erupts at delivery.

[[jim-highsmith]]'s [[adaptive-software-development]] addressed this directly through its "speculate, collaborate, learn" cycle: "speculate" rather than "plan" because the framing encodes the appropriate epistemic humility. The Agile response is not to abandon planning — principle 2 of the [[agile-manifesto-twelve-principles]] says "welcome changing requirements," not "don't plan" — but to change the relationship to the plan.

## Intellectual Connections

**[[empirical-process-control]]** provides the theoretical framework: software development is an empirical process in which inspection of actual outputs routinely reveals that the original plan was wrong. Adaptation is not a failure; it is the mechanism.

**[[inspect-and-adapt]]** is the operational implementation: the short iteration cycle creates regular inspection points where the plan can be updated based on what was learned. The Sprint Review is explicitly an opportunity to update the Product Backlog — i.e., to respond to change.

**The lean concept of "last responsible moment"** is a decision-timing principle that converges with this value: delay commitment decisions until you have enough information to make them well, because early commitments made under uncertainty are frequently wrong and costly to reverse. This is a structural argument for the Agile approach to requirements.

**Lean startup's Build-Measure-Learn loop** — developed by Eric Ries building on the Agile tradition — is an extension of the same principle into product strategy: treat every product decision as a hypothesis, measure its outcome, and adapt.

## The [[iron-triangle]] Connection

Conventional project management treated scope, time, and cost as the three constrained variables, with scope fixed and time/cost allowed to vary (or some combination of two of the three fixed). Agile inverts this: fix time (the iteration) and cost (the team), and allow scope to vary. Responding to change is only possible if scope is variable; fixed-scope contracts make responsiveness impossible by design. This is why "customer collaboration over contract negotiation" is a companion value — contracts that fix scope are organizational structures that prevent responding to change.

## Reception

The value has been criticized from both directions. Those committed to traditional project management argue that stakeholders require predictability and that variable scope undermines accountability. Post-Agile critics note that in many enterprise Agile implementations, the plan is still treated as a commitment (at the PI level in [[safe-scaled-agile-framework]], for example), making the value aspirational rather than operational.
