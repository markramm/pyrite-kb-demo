---
id: deictic-representation
title: "Deictic Representation"
type: concept
first_appeared: "1988 — PhD dissertation; 'Pengi' system"
key_writings:
  - pengi-implementation-of-a-theory-of-activity
key_concepts:
  - grammars-of-action
importance: 8
research_status: draft
links:
  - target: pengi-implementation-of-a-theory-of-activity
    relation: developed_in
    kb: red-rock-eater
  - target: grammars-of-action
    relation: related_to
    kb: red-rock-eater
  - target: hubert-dreyfus
    relation: influenced_by
    note: Heidegger's ready-to-hand via Dreyfus
    kb: red-rock-eater
tags:
  - ai
  - representation
  - situated-action
  - pengi
  - planning-critique
---

## Overview

Deictic representation is Agre's alternative to the classical AI approach of representing the world through objective, context-independent descriptions. Drawing on the linguistic concept of deixis (words like "this," "here," "now" whose meaning depends on context), Agre proposed representing the world in terms of the agent's ongoing, situated relationship to its environment rather than through a detached, God's-eye model.

In classical AI planning, an agent builds a model of the world using objective identifiers — "block A is on block B." In deictic representation, the world is described in terms of functional relationships to the agent's current activity — "the thing I'm reaching for," "the obstacle in my path." This approach was implemented in the Pengi system, a program that played the arcade game Pengo using deictic representations rather than planning.

## Significance

Deictic representation was both a technical contribution and a philosophical argument. Technically, it showed that sophisticated behavior could emerge without the kind of elaborate world-modeling that planning-based AI required. Philosophically, it drew on phenomenological critiques of representationalism (particularly Heidegger's analysis of ready-to-hand vs. present-at-hand) to argue that the planning paradigm reflected bad philosophy rather than good engineering.
