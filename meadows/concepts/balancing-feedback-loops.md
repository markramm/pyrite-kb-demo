---
id: balancing-feedback-loops
title: "Balancing Feedback Loops"
type: concept
importance: 8
tags:
- system-dynamics
- negative-feedback
- equilibrium
- regulation
first_appeared: "Industrial Dynamics (Forrester, 1961)"
source_tradition: system dynamics
key_writings:
- thinking-in-systems-2008
- places-to-intervene-in-a-system-1997
related_concepts:
- feedback-loops
- reinforcing-feedback-loops
- delays-in-systems
- leverage-points
- stocks-and-flows
- resilience
research_status: draft
---

A balancing feedback loop (also called a negative feedback loop) is a loop in which a change in a stock generates a corrective response that opposes the original change. The system senses a gap between its current state and some goal or reference level, and acts to close that gap. Balancing loops are the mechanism of regulation, homeostasis, and goal-seeking behavior.

The label "negative" again does not mean bad — it means that the feedback signal has the opposite sign from the change that created it, pushing back against deviation. A thermostat is the canonical example: room temperature falls below the set point, the furnace turns on, temperature rises back toward the set point, the furnace turns off. The body's regulation of blood sugar, a central bank adjusting interest rates to target inflation, a predator population expanding when prey become abundant and contracting when prey become scarce — all are balancing loops.

Meadows represented balancing loops with a B (or a - symbol circling the loop). The key structural feature is a **goal**: every balancing loop has an implicit or explicit reference level toward which the system is being driven. This insight is practically significant because it means that changing the goal of a balancing loop — the reference point against which the gap is measured — is a high-leverage intervention. In her [[leverage-points]] hierarchy, changing goals ranks at level 3 (very high leverage).

Balancing loops produce stable, goal-seeking behavior only when they work well. They are disrupted in two main ways. First, [[delays-in-systems]]: when the feedback signal arrives late, the corrective action overshoots and the system oscillates around its goal rather than settling smoothly. The classic illustration is the shower that swings between too hot and too cold because the temperature feedback lags behind the adjustment. Second, weak feedback: if the information signal reaching the decision-maker is distorted, delayed, or absent, the gap between actual state and goal may not be perceived and no correction occurs. Meadows argued that many environmental failures are cases of weak balancing feedback — the signals (ecosystem degradation, climate change) arrive slowly and indirectly while the reinforcing loops driving economic growth remain strong and fast.

Balancing loops are also subject to policy resistance. When an external intervention tries to change a stock, the balancing loops within the system act to restore the original state. Drug enforcement efforts reduce drug supply; prices rise; profits for suppliers increase; supply is restored. This is the "fixes that fail" pattern — interventions that work temporarily but trigger compensating feedbacks that cancel the effect.

Understanding which balancing loops are active in a system, what their goals are, and whether those goals match human intentions is central to Meadows's diagnostic approach to systems. A system will always serve its actual goals, not the goals observers assume it has. Discovering the true goals embedded in a system's structure — through [[bounded-rationality-in-systems]] and [[iceberg-model]] analysis — was for Meadows both an analytical and an ethical task.
