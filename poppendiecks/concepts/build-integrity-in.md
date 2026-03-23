---
id: build-integrity-in
title: Build Integrity In
type: concept
tags:
- lean-software-development
- seven-lean-principles
- quality
- architecture
- tps-translation
links:
- target: poka-yoke
  relation: translates
  note: Building quality in through error-prevention, from Shingo's poka-yoke
  kb: tps
- target: jidoka
  relation: translates
  note: Building quality in from TPS jidoka (automation with a human touch)
  kb: tps
importance: 8
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: jidoka (built-in quality, automation with a human touch); poka-yoke (mistake-proofing)
  — Shigeo Shingo
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- seven-lean-principles
- eliminate-waste
- empower-the-team
- decide-as-late-as-possible
- optimize-the-whole
research_status: draft
---

Build integrity in is Principle 6 of the [[seven-lean-principles]], introduced by [[mary-poppendieck]] and [[tom-poppendieck]] in [[lean-software-development-agile-toolkit-2003]]. Its TPS sources are *jidoka* (built-in quality, sometimes translated as "automation with a human touch") and [[shigeo-shingo]]'s *poka-yoke* (mistake-proofing) — the cluster of TPS methods that treat quality as a design property rather than an inspection outcome.

## Two Dimensions of Integrity

The Poppendiecks distinguish two dimensions of software integrity:

**Perceived integrity** is the customer's experience of the system — whether it does what they need, behaves consistently, responds intuitively, and builds trust through reliability. Perceived integrity is about the fit between the system and its users' actual needs and mental models. A system with high perceived integrity feels coherent and purposeful from the outside.

**Conceptual integrity** is the internal coherence of the system's design — whether its components share consistent assumptions, its architecture reflects a unified design philosophy, and its abstractions are well-chosen. A system with high conceptual integrity is easy to understand, modify, and extend, because every part of it reflects the same set of principles.

Fred Brooks in *The Mythical Man-Month* argued that conceptual integrity was the most important property of a software system, and that it was best achieved by limiting the number of architects making fundamental design decisions. The Poppendiecks agree on the importance but disagree on the mechanism: they argue that built-in quality practices — refactoring, test-driven development, continuous integration — can maintain conceptual integrity in a distributed team without requiring a single architect's control.

## The TPS Foundation: Jidoka and Poka-Yoke

[[taiichi-ohno]]'s *jidoka* principle held that machines should be designed to stop automatically when they detect a defect, rather than continuing to produce defective output. This was one of TPS's two pillars (alongside just-in-time). The implication is that quality is built into the production system itself — not inspected in afterward.

[[shigeo-shingo]] developed *poka-yoke* (mistake-proofing) as the engineering discipline for jidoka: designing processes and tools so that defects are either impossible or immediately detectable. Poka-yoke is not just error detection; it is error prevention by design.

## Translation to Software

The Poppendiecks translated jidoka and poka-yoke into software quality practices. The software equivalents of mistake-proofing include:

- **Test-driven development (TDD):** Writing tests before code makes defects immediately detectable and builds a regression safety net that enables confident refactoring.
- **Continuous integration:** Integrating code continuously catches integration defects as soon as they are introduced, rather than accumulating them into large integration episodes.
- **Refactoring:** Maintaining code quality through ongoing structural improvement, rather than allowing technical debt to accumulate until it becomes unmanageable.
- **Automated builds:** Automating compilation, testing, and deployment reduces the manual error surface in the delivery process.

These practices align with [[kent-beck]]'s Extreme Programming practices, which the Poppendiecks explicitly acknowledged. The lean framework provided a theoretical grounding for why XP practices work: they are engineering implementations of built-in quality.

## Integrity and the Last Responsible Moment

Build integrity in is the complement to [[decide-as-late-as-possible]]. Deferring decisions preserves optionality; building integrity in ensures that deferral does not accumulate into chaos. A codebase maintained through ongoing refactoring and continuous testing is a codebase that remains malleable enough to incorporate late decisions. Without integrity-building disciplines, deferred decisions pile up as technical debt that eventually makes the system fragile.

[[shigeo-shingo]]'s contribution is important here: mistake-proofing is not just reactive (catching defects) but prospective (designing so defects cannot occur). The equivalent in software is designing systems with clean interfaces, clear abstractions, and explicit contracts — architecture choices that make certain classes of error structurally impossible.
