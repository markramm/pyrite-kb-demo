---
id: fast-feedback
title: "Fast Feedback"
type: concept
tags:
- feedback
- learning
- cycle-time
- economics
- iteration
links:
- target: tempo
  relation: related_to
  note: Reinertsen's fast feedback principle parallels Boyd's tempo concept — both argue that the rate of cycling through observe-decide-act (or build-measure-learn) is the critical competitive variable
  kb: boyd
importance: 7
metadata:
  first_appeared: "managing-the-design-factory"
  key_writings: &id001
  - managing-the-design-factory
  - principles-of-product-development-flow
  related_concepts: &id002
  - batch-size-reduction
  - managing-variability
  - cost-of-delay
  - flow-control
  research_status: draft
first_appeared: "managing-the-design-factory"
key_writings: *id001
related_concepts: *id002
research_status: draft
---

Fast feedback is the principle that accelerating the speed of learning loops — the time between an action and information about its consequences — is economically valuable and should be actively managed. In Reinertsen's framework, this is not primarily a cultural principle about psychological safety or iteration mindset, but an economic argument about the compounding cost of delayed error correction.

## The Economic Argument

Every product development effort is an information problem: the team makes decisions based on assumptions (about user needs, technical feasibility, market conditions) and eventually receives feedback about whether those assumptions were correct. If an assumption is wrong, the cost of correction depends on how much work was built on that assumption before the error was discovered.

Feedback delay is the time between making a false assumption and learning it is false. During that delay, work accumulates on a flawed foundation. The correction cost grows with the amount of accumulated work, which grows with the feedback delay. This creates a compounding relationship: longer feedback delay → more accumulated rework → higher correction cost. The relationship is roughly linear for most development work — each additional week of feedback delay costs approximately one additional week of rework.

This cost is a specific instance of [[cost-of-delay]]: the delay in receiving feedback has a per-unit-time cost equal to the rework rate accumulated on the flawed assumption.

## Connection to Batch Size

[[batch-size-reduction]] is the primary operational mechanism for accelerating feedback. Smaller batches complete and reach validation faster. In a test-code cycle, smaller test batches mean faster cycles. In a release cycle, smaller releases mean faster market feedback. In a design cycle, smaller design increments mean faster usability feedback.

The connection is structural: batch size determines how much work is processed before integration and feedback; smaller batches mean more frequent integration and faster feedback.

## Managing Variability of Feedback

Not all feedback is equally useful — the value of feedback depends on its signal-to-noise ratio and its timeliness. [[managing-variability]] connects here: high variability in feedback (noisy signals, inconsistent user responses, variable test results) reduces the economic value of fast feedback because more samples are needed to extract a reliable signal. Managing variability in the development process increases the value of each feedback cycle.

## Historical Lineage

Fast feedback is central to several traditions that Reinertsen engages with:

- [[w-edwards-deming]]'s Plan-Do-Check-Act (PDCA) cycle is explicitly a fast feedback mechanism applied to quality improvement — the shorter the PDCA cycle, the faster the learning
- Boyd's OODA loop (Observe-Orient-Decide-Act) is a decision feedback cycle whose speed determines competitive advantage in fast-moving environments
- Scientific method generally: hypothesis-experiment-observation cycles, where faster cycles accelerate learning

Reinertsen's contribution is expressing the value of fast feedback in economic terms — attaching a dollar cost to feedback delay — rather than as a philosophical commitment to learning or a cultural value.

## Practical Manifestations

Fast feedback prescriptions include: automated testing (reduces test cycle time from days to minutes), continuous integration (reduces integration feedback from weeks to hours), minimum viable products (reduces market feedback from full-product cycles to early-stage validation), and short-cycle design reviews (reduces design feedback from phase-end reviews to weekly or daily check-ins).
