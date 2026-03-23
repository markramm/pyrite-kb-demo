---
id: eliminate-waste
title: Eliminate Waste
type: concept
tags:
- lean-software-development
- seven-lean-principles
- waste
- tps-translation
links:
- target: seven-wastes-muda
  relation: translates
  note: Software waste elimination principle derived from TPS muda
  kb: tps
- target: muri-and-mura
  relation: builds_on
  note: Ohno's fuller waste framework — overburden and unevenness alongside muda
  kb: tps
importance: 9
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: muda (seven wastes of manufacturing) — Taiichi Ohno
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- seven-lean-principles
- seven-wastes-of-software
- amplify-learning
- value-stream-mapping-for-software
- optimize-the-whole
research_status: draft
---

Eliminate waste is Principle 1 of the [[seven-lean-principles]] framework that [[mary-poppendieck]] and [[tom-poppendieck]] introduced in [[lean-software-development-agile-toolkit-2003]]. It is the most direct translation from the Toyota Production System: [[taiichi-ohno]]'s foundational insight that manufacturing processes are riddled with non-value-adding activities, and that removing them is the primary lever for improving both quality and speed.

## The TPS Foundation

[[taiichi-ohno]] identified seven categories of manufacturing waste (*muda*): overproduction, waiting, transport, overprocessing, inventory, motion, and defects. His framework at Toyota was radical because it argued that most of what happens in a factory — movement of materials, inspection steps, inventory buffers — adds cost without adding value. Elimination of waste, not optimization of individual operations, was the path to competitive advantage.

[[shigeo-shingo]] reinforced this insight by distinguishing between work (value-adding) and waste (non-value-adding), and developed specific techniques — particularly *poka-yoke* (mistake-proofing) — to eliminate defects at their source rather than catching them downstream.

## Translation to Software

The Poppendiecks recognized that software development contains analogous waste categories, but the translation is not one-to-one. In manufacturing, waste is visible: excess inventory sits on shelves, unnecessary transport is physically observable. In software, waste is largely invisible — it hides in requirements documents no one reads, code that is written but never shipped, and meeting cycles that produce no decisions.

The seven software wastes are detailed in [[seven-wastes-of-software]]. The most important translation difference is that software waste is primarily *cognitive* rather than physical. Partially done work wastes not floor space but working memory and context. Handoffs lose not physical materials but tacit knowledge. This cognitive character of software waste makes it harder to see — which is why [[value-stream-mapping-for-software]] is necessary to make the waste visible.

## "See the Waste"

The Poppendiecks frame waste elimination as a two-step discipline: first, learn to *see* waste (using tools like value stream mapping); second, systematically remove it. They argue that most software teams are surrounded by waste they have normalized — long requirements phases, multi-stage approval processes, large release batches — and that making these visible is itself a significant intervention.

This connects to [[amplify-learning]]: the ability to see waste is itself a learned skill. Teams that are poor at identifying waste are teams that have not yet learned to distinguish value-adding from non-value-adding work. Waste elimination and learning amplification are therefore not separate activities but mutually reinforcing disciplines.

## Relationship to Agile Practices

Many agile practices can be understood as waste-elimination techniques. User stories eliminate the waste of requirements documents that misrepresent customer needs. Continuous integration eliminates the waste of deferred integration and the defects it hides. Daily standups reduce the waste of delayed communication. The Poppendiecks' contribution was to give these practices a theoretical foundation — not just "this works" but "this works because it eliminates a specific category of waste."

[[optimize-the-whole]] provides the systemic constraint on waste elimination: removing waste from one step while ignoring system-level flow can create new bottlenecks elsewhere. Waste elimination done well is always done in the context of whole-system performance.
