---
id: critical-chain-project-management
title: Critical Chain Project Management
type: concept
tags:
- project-management
- scheduling
- buffer-management
links:
- target: wip-constraints
  relation: related_to
  note: Critical chain addresses project multitasking and buffers in ways that parallel
    Reinertsen's WIP constraints for product development flow
  kb: reinertsen
importance: 8
first_appeared: Critical Chain (1997)
key_writings:
- critical-chain
- goldratt-satellite-program
related_concepts:
- theory-of-constraints
- five-focusing-steps
- buffer-management
- drum-buffer-rope
- thinking-processes
research_status: draft
---

Critical Chain Project Management (CCPM) applies [[theory-of-constraints]] to project scheduling, addressing the chronic failure of projects to complete on time, within scope, and on budget. [[eliyahu-goldratt]] introduced CCPM in the business novel [[critical-chain]] (1997), set in a university MBA program, making it the most complete published statement of his ideas on project management.

The conventional critical path method (CPM) embeds safety time within individual task estimates: each person adds padding to their own estimate to protect against uncertainty. This produces several pathological behaviors that Goldratt identified: Parkinson's Law (work expanding to fill available time), the student syndrome (delaying start until the deadline approaches), and multitasking across projects — each of which consumes the embedded safety without providing protection at the project level.

CCPM's solution is to strip the safety time out of individual task estimates, consolidate it into project-level and feeding buffers, and then use [[buffer-management]] to signal when the project needs attention. The "critical chain" is the longest chain of dependent tasks accounting for both task dependencies and resource dependencies — the constraint of the project. A project buffer sits at the end of the critical chain to protect the commitment date.

Feeding buffers protect the critical chain from delays in non-critical paths. Resource buffers alert key resources before they are needed. These buffers replace task-level padding and provide a single, visible indicator of project health.

In multi-project environments, CCPM identifies the constraint resource across all projects (the drum), staggers project starts to avoid overloading it, and uses fever charts derived from buffer management to prioritize where attention should go. This multi-project application extended [[drum-buffer-rope]] logic into the project domain and was developed further by [[eli-schragenheim]] and practitioners in the [[avraham-y-goldratt-institute]] network.
