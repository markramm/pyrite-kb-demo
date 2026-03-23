---
id: buffer-management
title: Buffer Management
type: concept
tags:
- monitoring
- flow-management
- scheduling
links:
- target: managing-variability
  relation: related_to
  note: Both address how to absorb variability in a flow system without blocking throughput
  kb: reinertsen
importance: 7
first_appeared: The Race (1986); developed through multiple books
key_writings:
- the-race
- theory-of-constraints-book
- critical-chain
related_concepts:
- drum-buffer-rope
- critical-chain-project-management
- five-focusing-steps
- theory-of-constraints
- throughput-accounting
research_status: draft
---

Buffer Management is the ongoing monitoring discipline within [[theory-of-constraints]] that uses the consumption of time or inventory buffers as the primary signal for managerial attention. Rather than tracking individual machine utilization or task completion percentages, Buffer Management directs focus to where the system's protective capacity is being eroded — providing an early warning before the constraint or a project commitment date is actually jeopardized.

In the [[drum-buffer-rope]] production context, a time buffer sits in front of the constraint. Buffer Management divides this buffer into three zones — green, yellow, and red — based on how much buffer remains. Work arriving in the green zone requires no action; yellow signals monitoring; red signals that expediting or intervention may be needed. The key insight is that most problems will be resolved naturally before they reach red, so managers spend attention where it is genuinely needed rather than reacting to every local perturbation.

Buffer Management evolved alongside DBR through [[the-race]] (1986) and was formalized in [[theory-of-constraints-book]] (1990). [[eliyahu-goldratt]] extended it into project management in [[critical-chain]] (1997), where it became the "fever chart" — a visual tool mapping buffer consumption against project completion percentage. A fever chart moving up and to the right signals a project in trouble; one moving down and to the right signals healthy buffer recovery.

The discipline resolves a key tension in subordination (step 3 of [[five-focusing-steps]]): subordinating non-constraint resources to the constraint's pace means non-constraint resources will sometimes be idle, which looks wasteful by traditional metrics. Buffer status provides a legitimate alternative metric — managers protect and manage buffer consumption rather than machine utilization, aligning measurement with system-level performance.
