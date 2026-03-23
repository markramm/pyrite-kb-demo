---
id: delays-in-systems
title: Delays in Systems
type: concept
tags:
- system-dynamics
- time-lags
- oscillation
- policy-resistance
links:
- target: the-funnel-experiment
  relation: related_to
  note: Deming's funnel experiment shows how reacting to noise (ignoring delays) makes
    systems worse — illustrates Meadows's delay dynamics
  kb: deming
- target: drum-buffer-rope
  relation: related_to
  note: Buffers in DBR explicitly account for delays and variability; Meadows's delay
    analysis explains why buffers are necessary
  kb: goldratt
- target: critical-chain-project-management
  relation: related_to
  note: Critical chain addresses delays in project systems through feeding buffers
    and project buffers
  kb: goldratt
- target: batch-size-reduction
  relation: related_to
  note: Large batches create delays through queue accumulation; reducing batch size
    reduces delays — Meadows's delay dynamics in action
  kb: reinertsen
- target: queueing-theory-applied
  relation: related_to
  note: Queuing theory quantifies how delays grow nonlinearly with utilization; formalizes
    Meadows's insight that delays destabilize systems
  kb: reinertsen
- target: batch-size-death-spiral
  relation: related_to
  note: Death spiral is a reinforcing feedback loop where delays cause larger batches
    which cause more delays — classic Meadows positive feedback trap
  kb: reinertsen
importance: 8
first_appeared: Industrial Dynamics (Forrester, 1961)
source_tradition: system dynamics
key_writings:
- thinking-in-systems-2008
- groping-in-the-dark-1982
- limits-to-growth-1972
related_concepts:
- feedback-loops
- balancing-feedback-loops
- reinforcing-feedback-loops
- stocks-and-flows
- overshoot-and-collapse
- bounded-rationality-in-systems
research_status: draft
---

Delays are time lags between a cause and its effect — between an action and the response to that action, or between a change in a stock and the signal that registers that change in a feedback loop. They are among the most common sources of system misbehavior: oscillation, overshoot, policy resistance, and persistent mismanagement all frequently trace to delays that are longer than the decision-makers acting on feedback realize.

Meadows treated delays as one of the most practically important structural features a systems thinker must learn to recognize. The reason is counterintuitive: a system with delays does not simply produce the same behavior more slowly. It produces qualitatively different behavior. A balancing loop without delay seeks its goal smoothly. The same loop with a long delay oscillates — the corrective action overshoots because it was calibrated to a state that no longer exists by the time the action takes effect.

The shower metaphor Meadows used repeatedly: you turn the knob toward hot, the water takes a few seconds to change temperature, you keep turning toward hot because it's still cold, and suddenly you are scalded — at which point you overcorrect toward cold. The loop seeks room temperature but produces an oscillating series of burns and chills. The fix is not faster action but slower, more patient action — understanding the delay and waiting for it to resolve before adjusting again.

In [[limits-to-growth-1972]], delays were central to the world model's dynamics. The delay between resource consumption and recognition of scarcity, the delay between industrial pollution and ecosystem response, the delay between declining living standards and reduced birth rates — these were the mechanisms that allowed the world system to overshoot carrying capacity before feedback could redirect it. [[overshoot-and-collapse]] is fundamentally a delay-driven phenomenon: a reinforcing growth loop runs past the point where a balancing resource-limit loop could check it, because the signal arrives too late.

Meadows identified several types of delay in systems. **Material delays** occur in physical flows: trees take decades to grow; a ship takes years to build. **Information delays** occur in the signals that reach decision-makers: market prices reflect past supply and demand; scientific evidence about environmental damage takes years to accumulate and more years to translate into policy. **Perception and response delays** are cognitive and institutional: people resist updating mental models; organizations take time to authorize new approaches; policy implementation lags behind policy decisions.

The [[bounded-rationality-in-systems]] problem compounds delays. Decision-makers acting on delayed, incomplete information make choices that seem rational given what they know. The aggregate result of many such individually rational choices can be collectively irrational — the Beer Game simulation, developed at [[mit-system-dynamics-group]], demonstrates how supply chain oscillations are produced by the delays and limited information facing each player, even when all players are trying to optimize.

Meadows's practical prescription: when you find oscillation in a system, look for delays. When you find overshoot, look for delayed feedback. And when designing interventions, ask whether you are creating new delays or whether you can shorten existing ones. Faster feedback — reducing the delay between action and consequence — is a moderately high leverage intervention in her [[leverage-points]] framework. But she cautioned that speeding up feedback loops that are already fast enough can itself cause oscillation; the goal is appropriate timing, not maximum speed.
