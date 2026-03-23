---
id: seven-lean-principles
title: Seven Lean Principles
type: concept
tags:
- lean-software-development
- framework
- tps-translation
- core-principles
links:
- target: deming-s-place-in-the-lean-lineage
  relation: builds_on
  note: Deming is a foundational ancestor in the lean lineage
  kb: deming
importance: 10
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: Toyota Way principles (Liker's 14 points; TPS house of waste elimination
  and respect for people)
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
- leading-lean-software-development-2009
related_concepts:
- eliminate-waste
- amplify-learning
- decide-as-late-as-possible
- deliver-as-fast-as-possible
- empower-the-team
- build-integrity-in
- optimize-the-whole
- learning-not-results
research_status: draft
---

The seven lean principles are the organizing framework that [[mary-poppendieck]] and [[tom-poppendieck]] introduced in [[lean-software-development-agile-toolkit-2003]] to translate the Toyota Production System into software development practice. The framework gives lean software development its intellectual backbone and distinguishes it from other agile methods by grounding each principle in a specific manufacturing antecedent.

## The Seven Principles

1. **[[eliminate-waste]]** — Remove anything that does not add value from the customer's perspective. In TPS, this maps to Taiichi Ohno's concept of *muda* (waste), which [[taiichi-ohno]] classified into seven types. The Poppendiecks translated these into seven software-specific wastes.

2. **[[amplify-learning]]** — Software development is a learning process. The primary output is not code but knowledge. This is the Poppendiecks' most original contribution — it reframes what a software value stream actually produces.

3. **[[decide-as-late-as-possible]]** — Delay irreversible decisions until the last responsible moment. In TPS, this maps to set-based concurrent engineering developed by Allen Ward at Toyota. Deferring commitment preserves optionality when information is still emerging.

4. **[[deliver-as-fast-as-possible]]** — Compress cycle time to accelerate learning and reduce risk. This maps to pull systems and just-in-time delivery in TPS. [[donald-reinertsen]]'s queueing theory provides the mathematical foundation for why speed matters.

5. **[[empower-the-team]]** — Push decision-making authority down to the people doing the work. In TPS, this is the "respect for people" pillar — workers who understand the process are best positioned to improve it.

6. **[[build-integrity-in]]** — Quality is not inspected in at the end; it is designed in from the start. This maps to Shigeo Shingo's *poka-yoke* (mistake-proofing) and the TPS principle that every worker is responsible for quality.

7. **[[optimize-the-whole]]** — Optimize the entire value stream, not individual steps. Local optimization — making one component faster or more efficient — routinely degrades system-level performance. This is the systems-thinking pillar of lean.

## TPS Antecedents

The framework draws directly from [[taiichi-ohno]]'s waste elimination framework, [[shigeo-shingo]]'s quality-at-source methods, and [[w-edwards-deming]]'s system of profound knowledge. [[james-womack]] and [[daniel-jones]] had already synthesized TPS into a transferable framework in *The Machine That Changed the World* (1990) and *Lean Thinking* (1996). The Poppendiecks' contribution was the next translation step: applying that synthesized lean thinking to the specific characteristics of software, where the product is intangible, duplication is free, and the primary constraint is human knowledge rather than physical throughput.

## What Changed in Translation

The most significant adaptation is Principle 2 — amplifying learning. In manufacturing, value is embodied in the physical product moving through the value stream. In software, the equivalent is the knowledge embedded in the team and codebase. This means waste, flow, and optimization all look different. Eliminating waste in software means eliminating activities that impede learning, not merely activities that slow physical throughput. This reorientation runs through all seven principles and is what makes lean software development more than a superficial mapping of manufacturing metaphors.

The seven principles were elaborated across all three books in the Poppendiecks' trilogy. [[implementing-lean-software-development-2006]] deepened the implementation guidance for each principle, and [[leading-lean-software-development-2009]] addressed how organizational leadership either enables or undermines the framework.
