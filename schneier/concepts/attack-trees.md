---
id: attack-trees
title: Attack Trees
type: concept
tags:
- technical
- methodology
- threat-modeling
- formal-methods
links:
- target: current-reality-tree
  relation: related_to
  note: Attack trees and Goldratt's current-reality trees are both structured cause-and-effect
    diagrams for reasoning about complex failure pathways
  kb: goldratt
importance: 8
first_appeared: '1999'
key_writings:
- schneier-on-security-book
- secrets-and-lies
related_concepts:
- threat-modeling
- security-mindset
- security-is-a-process
- security-economics
research_status: draft
---

Attack trees are a formal, hierarchical methodology for modeling how attackers can compromise a system. Schneier introduced the technique in a 1999 paper published in Dr. Dobb's Journal and subsequently developed it in [[secrets-and-lies]] and [[schneier-on-security-book]]. The method represents an attempt to apply systematic, rigorous thinking to the adversarial analysis that the [[security-mindset]] requires — translating an intuitive cognitive practice into a sharable, actionable engineering tool.

## Structure of the Method

An attack tree is a tree-structured diagram in which:

- The **root node** represents the attacker's goal (e.g., "gain unauthorized access to the database")
- **Child nodes** represent sub-goals or alternative approaches to achieving the parent goal
- **Leaf nodes** represent basic attack steps — actions that can be assessed for feasibility, cost, and probability
- **AND nodes** represent steps that must all be completed (sequential dependencies)
- **OR nodes** represent alternative paths (any one of which achieves the goal)

This structure makes the model compositional: sub-trees can be reused across different threat analyses, and the tree as a whole makes explicit every path by which an attacker might reach their objective.

## Analytical Value

The tree structure supports several types of analysis:

**Completeness checking.** By requiring that all paths to an objective be represented, attack trees force analysts to articulate what they know about an attacker's option space. Gaps in the tree reveal gaps in understanding.

**Prioritization.** Each leaf node can be annotated with attributes — cost to the attacker, technical difficulty, detectability, probability of success. These annotations can be propagated up the tree (using AND/OR logic) to assess entire attack paths. This makes [[security-economics]] tractable: security investment can be directed toward the most plausible, lowest-cost paths.

**Communication.** Trees are visual and navigable; they make threat analysis communicable to non-technical stakeholders in a way that prose descriptions rarely are.

**Attack surface mapping.** The tree makes explicit which components of a system appear in attack paths, producing a natural definition of the attack surface — the set of points at which an adversary can interact with the system.

## Context in Schneier's Work

Attack trees were Schneier's primary contribution to formal threat analysis methodology. They emerged from his frustration with security analysis that was either too vague to be actionable or so narrowly technical that it missed the human and organizational dimensions of actual attacks. The attack tree formalism accommodates both: leaf nodes can represent technical steps (exploit a buffer overflow) or human steps (bribe an employee) with equal facility.

The methodology predates the formalization of [[threat-modeling]] as a software engineering discipline, but feeds directly into it. [[adam-shostack]], who developed Microsoft's threat modeling approach (STRIDE/DREAD) and wrote the definitive textbook on threat modeling, cites attack trees as an important precursor and complementary technique.

Schneier developed attack trees in the same intellectual moment as [[secrets-and-lies]] — both represent the shift from treating security as a purely cryptographic/mathematical problem to treating it as a systems problem requiring adversarial analysis of human-technical assemblies.

## Limitations

Attack trees have known limitations that Schneier and subsequent researchers have acknowledged:

**Combinatorial complexity.** Realistic systems generate trees with enormous numbers of paths. Managing this complexity requires judgment about which threats are worth modeling, which reintroduces the analyst's assumptions back into what was meant to be a systematic method.

**Static representation.** Attack trees capture a point-in-time analysis. They do not naturally represent the dynamic nature of real attacks — the way adversaries adapt as defenses change — though extensions to the formalism have addressed this.

**False completeness.** A tree can look complete while missing important attack categories. The methodology provides structured discipline but does not guarantee that the analyst has imagined all relevant attacks. This is a fundamental limitation of any anticipatory analysis against adaptive adversaries.

These limitations do not undermine the value of the technique — they are arguments for using it with appropriate epistemic humility, which is consistent with Schneier's broader stance on security methods. The [[security-is-a-process]] framework provides the context: attack trees are one tool in an ongoing analytical practice, not a one-time certification of security.

## Legacy

Attack trees have been adopted widely in industrial control systems security, formal verification research, and risk management frameworks. The formalism has been extended by researchers in computer science and operations research — some using probabilistic graphical models, others incorporating game-theoretic elements to model attacker-defender interactions. The core insight — that threat analysis should be systematic, adversarial, hierarchical, and annotatable — has become foundational to the security engineering field.
