---
id: optimize-the-whole
title: Optimize the Whole
type: concept
tags:
- lean-software-development
- seven-lean-principles
- systems-thinking
- suboptimization
- tps-translation
links:
- target: appreciation-for-a-system
  relation: influenced_by
  note: Deming's first SoPK component directly supports optimize-the-whole
  kb: deming
- target: management-by-objectives-deming-s-critique
  relation: builds_on
  note: Deming's critique of local optimization informs optimize-the-whole
  kb: deming
- target: theory-of-constraints
  relation: related_to
  note: Complementary system optimization frameworks
  kb: goldratt
- target: five-focusing-steps
  relation: related_to
  note: Goldratt's method for whole-system improvement
  kb: goldratt
- target: throughput-world-vs-cost-world
  relation: related_to
  note: Both frameworks argue against local cost optimization
  kb: goldratt
importance: 9
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: systems thinking; Toyota's value stream orientation; Deming's system of
  profound knowledge
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
- leading-lean-software-development-2009
related_concepts:
- seven-lean-principles
- eliminate-waste
- value-stream-mapping-for-software
- pull-systems-in-software
- learning-not-results
- amplify-learning
research_status: draft
---

Optimize the whole is Principle 7 of the [[seven-lean-principles]], introduced by [[mary-poppendieck]] and [[tom-poppendieck]] in [[lean-software-development-agile-toolkit-2003]]. Its TPS source is Toyota's fundamental value-stream orientation — the discipline of measuring and improving the *system's* performance rather than the performance of individual components — grounded in [[w-edwards-deming]]'s system of profound knowledge.

## The Suboptimization Problem

Suboptimization is the phenomenon in which improving the performance of a component degrades the performance of the system containing it. It is counterintuitive — surely making parts better makes the whole better — but it is pervasive and destructive in complex systems.

The classic manufacturing example is inventory buffers. A factory manager who optimizes a single machine's utilization — keeping it running at maximum capacity — will generate inventory buffers around that machine, because downstream processes cannot always consume its output immediately. That inventory is waste: it costs money, hides defects, and makes the overall system slower and less responsive, even though the machine itself is running at peak efficiency.

[[taiichi-ohno]] understood this: Toyota's pull system was designed precisely to prevent local optimization from degrading system flow. JIT and pull systems force the *system* to be the unit of optimization.

## Deming's Systems Thinking

[[w-edwards-deming]]'s System of Profound Knowledge identified systems thinking as one of four interrelated domains of knowledge necessary for improvement. His argument was that most management practice optimizes components rather than systems — rewarding individual performance while ignoring systemic interactions, setting departmental metrics that conflict with organizational goals, and attributing system-level problems to individual failures.

Deming's famous "red bead experiment" demonstrated that workers in a badly designed system will produce defects regardless of individual skill or effort, and that rewarding or punishing individuals for system-caused variation is both unfair and counterproductive. The right level of analysis is the system.

## Translation to Software

[[mary-poppendieck]] and [[tom-poppendieck]] applied this directly to software organizations. Common software suboptimizations include:

- **Developer utilization maximization:** Keeping developers 100% busy feels efficient but creates queues, delays context-switching costs, and eliminates the slack that enables learning and quality work.
- **Phase-based hand-offs:** Optimizing each phase of a waterfall process (requirements, design, coding, testing, deployment) while ignoring the costs of transitions between phases — information loss, rework, waiting — optimizes parts at the expense of the whole.
- **Team-level velocity metrics:** Measuring individual team throughput without measuring end-to-end delivery time creates local performance pressure that often slows the system.
- **Feature factory mentality:** Optimizing the rate of feature production without measuring whether features are actually used or whether they add system complexity that slows future development.

## Value Stream as the Unit of Optimization

The Poppendiecks argue, following [[james-womack]] and [[daniel-jones]]'s *Lean Thinking*, that the correct unit of optimization is the *value stream* — the entire sequence of activities from customer need to customer value. [[value-stream-mapping-for-software]] is the diagnostic tool that makes the whole value stream visible, enabling whole-system optimization.

This has organizational implications: functional silos (separate development, QA, operations, deployment teams) are optimized for departmental metrics rather than value stream metrics. [[gene-kim]]'s Three Ways of DevOps — Flow, Feedback, Continual Learning — are essentially the "optimize the whole" principle applied to the DevOps transformation, requiring organizational structures that align with the value stream rather than with functional departments.

## Connection to Learning Not Results

[[learning-not-results]] develops the deepest version of this insight: optimizing for result metrics — velocity, utilization, feature counts — is itself a form of local optimization that can degrade the system's long-run performance. A team that burns out its learning capacity in pursuit of short-term metrics is suboptimizing just as surely as the factory manager maximizing machine utilization. Whole-system optimization, on the Poppendiecks' account, must include the system's capacity for learning and adaptation over time.
