---
id: five-ideals
title: "The Five Ideals"
type: concept
importance: 6
tags:
- developer-experience
- gene-kim
- organizational-culture
- the-unicorn-project
first_appeared: "The Unicorn Project (Kim, 2019)"
key_writings:
- the-unicorn-project
related_concepts:
- three-ways
- software-delivery-performance
concept_type: framework
research_status: draft
---

The Five Ideals are the conceptual framework introduced in [[the-unicorn-project]] (2019) as a complement to [[three-ways]]. Where the Three Ways describes the system of work — how work should flow, how feedback should propagate, how learning should accumulate — the Five Ideals describe the developer experience within that system: what it feels like to work in a high-performing environment, and what conditions make that possible.

[[gene-kim]] developed the Five Ideals as a response to the developer-experience dimension that [[the-phoenix-project]] (2013) had underweighted. By 2019, the operational transformation story (deploy faster, reduce handoffs, eliminate the dev-ops wall) was established. The remaining frontier was understanding why developer work felt so miserable in many organizations even after DevOps adoption — and what a high-performing developer environment actually looked like from the inside.

## The Five Ideals

**First Ideal — Locality and Simplicity**: Teams should be able to make changes to their part of the system without requiring extensive coordination with other teams. Systems should be simple enough that developers can understand the consequences of their changes. The anti-pattern: a change to one service requires synchronized changes across ten other services, three approval queues, and two database migrations — requiring weeks of coordination for what should be a day of work. Locality means the blast radius of a change is small and predictable. Simplicity means the architecture does not impose cognitive overhead that obscures what a change does.

This ideal connects to the microservices architectural movement and to the "independently deployable" capability in [[accelerate-book]]'s 24 capabilities. It also connects to Conway's Law: if the team structure requires constant cross-team coordination, the architecture will reflect that coupling, making Locality impossible.

**Second Ideal — Focus, Flow, and Joy**: Developers should be able to spend most of their time doing development work — not navigating broken tooling, waiting for environments, resolving merge conflicts from long-lived branches, or fighting bureaucratic approval processes. Flow here references [[gene-kim]]'s use of Csikszentmihalyi's concept of flow state — the psychological condition of deep, uninterrupted engagement. Developer environments that interrupt constantly (slow builds, flaky tests, broken pipelines, unclear ownership) prevent flow states. Joy follows from flow: work that allows sustained focus is intrinsically motivating; work that consists of constant context-switching and firefighting is demoralizing.

The practical measurement: what percentage of developer time is spent on work that directly moves toward customer value, versus toil, rework, waiting, and bureaucracy? High-performing organizations maximize the former; low performers often invert the ratio.

**Third Ideal — Improvement of Daily Work**: Organizations should invest in improving the development environment and tooling, not just deliver features. Borrowing directly from the Toyota Production System: improving how we work is more important than the work itself. When teams cannot stop to improve because they are permanently in delivery mode, technical debt and tooling debt accumulate until the environment becomes a constraint on all other work.

This ideal maps directly to the Third Way ([[three-ways]]): continual learning and experimentation requires allocating time to improvement rather than treating it as a luxury contingent on feature delivery slack. The pattern in dysfunctional organizations: improvement is always scheduled for next quarter, after the current deadline, after the crisis passes. The crisis never passes.

**Fourth Ideal — Psychological Safety**: Teams need to be able to raise problems, propose experiments, and fail without fear of punishment. Kim draws explicitly on Amy Edmondson's research on psychological safety in teams — the finding that high-performing teams are not teams where no one makes mistakes, but teams where mistakes are surfaced, discussed, and learned from rather than concealed and repeated.

In DevOps terms: [[blameless-postmortems]] are the operational expression of psychological safety applied to incidents. When the response to a production failure is to find the responsible person and punish them, the organizational learning stops — future failures are concealed longer, surfaced less honestly, and repeated more often. When the response is to understand the system conditions that made failure possible, learning accumulates. Psychological safety is the cultural precondition for this response.

**Fifth Ideal — Customer Focus**: All work should be connected to customer value. The anti-pattern is completing work that is technically correct, delivered on time, and completely disconnected from what customers actually need. Customer Focus means teams understand who their customers are (internal or external), what those customers need, and how to validate that their work is meeting those needs. It connects DevOps to the broader product management and lean startup disciplines — the feedback loop from customer to product to developer to customer.

## Relationship to the Three Ways

The Five Ideals and the Three Ways are complementary frameworks, not competing ones:

- **Three Ways perspective**: systems, flow, feedback, learning — how work moves through the organization
- **Five Ideals perspective**: developer experience, architecture, culture, measurement at the individual and team level

The Five Ideals can be read as the developer-level conditions that enable the Three Ways to work. Locality enables flow (First Way) by reducing the coordination cost of each change. Focus, Flow, and Joy are the subjective experience of working in a well-designed First Way system. Improvement of Daily Work is the Third Way at the team level. Psychological Safety is the cultural prerequisite for honest Second Way feedback. Customer Focus connects the Second Way's feedback to actual user outcomes rather than system metrics.

## Adoption and Influence

The Five Ideals have achieved less practitioner adoption than the Three Ways. Several reasons:

1. The Three Ways were introduced in 2012-2013, when the DevOps movement was still crystallizing; they shaped the movement's self-understanding. The Five Ideals arrived in 2019, when practitioner vocabulary was already established.

2. The Three Ways are more directly actionable: each Way maps to specific practice categories. The Five Ideals are more evaluative — they describe states to achieve rather than practices to implement.

3. [[the-unicorn-project]] as a novel was less influential than [[the-phoenix-project]]; the audience for DevOps business fiction had saturated, and the Five Ideals did not generate the same management-level adoption as the Three Ways.

That said, the Second Ideal (Focus, Flow, and Joy) has influenced developer experience (DevEx) discussions, and the First Ideal (Locality and Simplicity) tracks closely with platform engineering discourse in the [[platform-engineering-era]].
