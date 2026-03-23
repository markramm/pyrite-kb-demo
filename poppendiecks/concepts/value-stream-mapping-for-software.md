---
id: value-stream-mapping-for-software
title: Value Stream Mapping for Software
type: concept
tags:
- lean-software-development
- value-stream
- process-analysis
- visualization
- tps-translation
links:
- target: value-stream
  relation: translates
  note: Software value stream mapping adapted from TPS value stream analysis
  kb: tps
importance: 6
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: value stream mapping (material and information flow mapping) — James Womack,
  Daniel Jones
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- eliminate-waste
- seven-wastes-of-software
- optimize-the-whole
- deliver-as-fast-as-possible
- pull-systems-in-software
research_status: draft
---

Value stream mapping for software is the Poppendiecks' adaptation of a lean manufacturing visualization tool — originally developed at Toyota and popularized by [[james-womack]] and [[daniel-jones]] — to the software delivery pipeline. Introduced in [[lean-software-development-agile-toolkit-2003]], it serves as the primary diagnostic tool for making invisible software waste visible, enabling teams to apply [[eliminate-waste]] and [[optimize-the-whole]] with precision rather than intuition.

## Manufacturing Origins

Value stream mapping was developed at Toyota as a way to visualize the complete flow of materials and information required to bring a product from raw material to customer. The technique was systematized and named by [[james-womack]] and [[daniel-jones]] in *Learning to See* (1998, with Mike Rother and John Shook), which made it accessible to non-Toyota manufacturers.

A value stream map documents every step in a process, the time each step takes, the time work waits between steps (queue time), and the type of activity (value-adding vs. non-value-adding). The resulting map typically reveals that value-adding activities — the steps that actually transform the product — represent a small fraction of total elapsed time. The rest is waiting, transport, inspection, and rework. In manufacturing, it is common to find that less than 5% of elapsed time is value-adding; the rest is waste.

## Translation to Software Delivery

[[mary-poppendieck]] and [[tom-poppendieck]] adapted value stream mapping to the software delivery pipeline — the sequence of activities from a customer need being identified to working software reaching the customer. The software value stream typically includes stages such as:

- Idea capture and prioritization
- Requirements analysis and specification
- Architecture and design
- Development (coding)
- Code review and integration
- Testing (unit, integration, acceptance)
- Deployment preparation
- Release and deployment
- Customer feedback

For each stage, a software value stream map records: How long does work sit waiting to enter this stage? How long does it actually take to process? What percentage of the work is done correctly the first time (versus requiring rework)?

## What Mapping Reveals

The Poppendiecks observed that software value stream maps tend to reveal the same surprise as manufacturing maps: the vast majority of elapsed time is waiting, not working. A feature that takes two weeks of actual development effort may take three months to reach production — not because coding is slow but because it waits in queues at multiple stages (waiting for review, waiting for a test environment, waiting for a deployment window, waiting for QA capacity).

This makes the case for [[deliver-as-fast-as-possible]] concrete: the path to faster delivery is not making developers work faster but removing the delays between steps. It also makes [[pull-systems-in-software]] actionable — the map shows exactly where work accumulates (where WIP is building up) and where pull system limits would be most effective.

## Identifying Waste Categories

Value stream maps can be annotated with [[seven-wastes-of-software]] categories, making the type of waste at each stage explicit:

- Long queue times between stages = **delays** (waste type 5)
- Rework loops = **defects** (waste type 7)
- Handoffs between teams = **handoff** waste (waste type 4)
- Multi-stage approval processes = **delays** and often **extra features** of governance overhead

This annotation turns a descriptive map into a diagnostic tool — not just "here is how long things take" but "here is what kind of waste is causing the delay and therefore which lean principle addresses it."

## Limitations of the Adaptation

The Poppendiecks acknowledged that the manufacturing-to-software translation of value stream mapping is imperfect. Software work is more variable and less repeatable than manufacturing work — no two features are identical, whereas manufactured parts are. The mapping tool must be used with awareness that it captures a snapshot of a variable process, not a fixed production line.

Nevertheless, value stream mapping proved influential in the DevOps movement, where the concept of "deployment pipeline" (Jez Humble and David Farley's *Continuous Delivery*, 2010) is essentially a value stream map of the software delivery process, optimized for flow through automation and pull. [[gene-kim]]'s DevOps transformation work uses value stream mapping explicitly as the diagnostic starting point for organizational improvement.
