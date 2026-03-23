---
id: five-focusing-steps
title: Five Focusing Steps
type: concept
tags:
- constraint-management
- process-of-ongoing-improvement
- operations
links:
- target: optimize-the-whole
  relation: related_to
  note: TOC's five focusing steps (identify the constraint, subordinate everything
    else) directly maps to Lean's optimize-the-whole principle
  kb: poppendiecks
importance: 10
first_appeared: The Goal (1984)
key_writings:
- the-goal
- theory-of-constraints-book
related_concepts:
- theory-of-constraints
- drum-buffer-rope
- buffer-management
- throughput-accounting
- throughput-world-vs-cost-world
research_status: draft
---

The Five Focusing Steps are the operational core of [[theory-of-constraints]] — a repeating managerial cycle that directs attention systematically to the factor most limiting a system's performance. [[eliyahu-goldratt]] first articulated them explicitly in [[theory-of-constraints-book]] (1990), though the underlying logic was already present in [[the-goal]] (1984) through the character of Alex Rogo's plant-floor discoveries.

The five steps are:

1. **Identify** the system's constraint — the single resource, policy, or factor that limits throughput.
2. **Exploit** the constraint — get maximum output from it without significant additional investment.
3. **Subordinate** everything else — align all non-constraint resources to support the constraint's pace, not their own local efficiency metrics.
4. **Elevate** the constraint — if throughput is still insufficient after exploitation and subordination, invest in increasing the constraint's capacity.
5. **Repeat** — once a constraint is broken, return to step one, because the constraint will have shifted.

The subordination step (step 3) is the most counterintuitive and the most frequently violated. Conventional management rewards local efficiency, which leads non-constraints to overproduce, creating excess inventory and masking the true constraint. [[drum-buffer-rope]] is the scheduling mechanism that operationalizes subordination in production environments, and [[buffer-management]] provides the ongoing monitoring signal.

The cycling nature of the process distinguishes TOC from one-time optimization. Goldratt called this the "process of ongoing improvement" (POOGI). The steps apply wherever a system has a goal — manufacturing, projects ([[critical-chain-project-management]]), supply chains, and beyond. The financial lens for evaluating each step's impact is provided by [[throughput-accounting]].
