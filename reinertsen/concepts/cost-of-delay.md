---
id: cost-of-delay
title: Cost of Delay
type: concept
tags:
- economics
- prioritization
- delay-cost
- flow
links:
- target: decide-as-late-as-possible
  relation: related_to
  note: Reinertsen's cost of delay quantifies what the Poppendiecks argue qualitatively
    — delaying decisions has an economic cost that must be weighed against the option
    value of waiting
  kb: poppendiecks
- target: throughput-accounting
  relation: related_to
  note: Reinertsen's cost of delay and Goldratt's throughput accounting are complementary
    economic lenses — both measure the economic impact of time on system performance
  kb: goldratt
importance: 10
first_appeared: managing-the-design-factory
key_writings:
- managing-the-design-factory
- principles-of-product-development-flow
related_concepts:
- economic-framework-for-prioritization
- weighted-shortest-job-first
- u-curve-optimization
- fast-feedback
research_status: draft
---

Cost of delay is the economic value lost per unit time by not having a feature, product, or capability in the market. It is the central quantitative instrument in [[economic-framework-for-prioritization]] and arguably the most important single concept in Reinertsen's body of work.

## The Core Logic

Most product development organizations track effort costs with precision — engineering hours, sprint points, headcount. They rarely quantify what it costs to be late. Reinertsen's insight, first articulated in [[managing-the-design-factory]] and refined extensively in [[principles-of-product-development-flow]], is that delay costs are just as real as effort costs, often larger, and almost always invisible.

Cost of delay answers the question: if this feature shipped one week later, what would that cost the business? The answer may be expressed as lost revenue per week, compounding market disadvantage, regulatory exposure, or strategic opportunity cost. Making that number explicit transforms prioritization from a political negotiation into an economic calculation.

## Why It Was Invisible

The invisibility of delay cost is structural. Effort appears on budgets and timecards. Delay appears nowhere on a balance sheet until the competitive consequences arrive — often months or years later and attributed to other causes. This asymmetry creates systematic bias toward over-investing in quality and scope while underweighting schedule. Reinertsen documented this bias through his consulting work across product development organizations and reported that only 15% of product developers know the cost of delay for their projects — making rational prioritization virtually impossible for the other 85%. He argued this invisibility was the primary source of poor prioritization decisions and the single most important thing an organization could fix.

## Economic Shape

Cost of delay is not a single number but a function of time. Different features have different profiles:

- **Urgent, time-decaying**: regulatory compliance with a hard deadline — cost of delay is near-zero before the deadline and catastrophic after
- **Linear**: a revenue-generating feature in a growing market — each week of delay costs approximately the same
- **Peaked**: a seasonal or event-driven feature — cost rises to a peak then falls as the opportunity passes

Understanding the shape of cost of delay, not just its magnitude, is necessary for correct scheduling decisions. This connects directly to [[weighted-shortest-job-first]], which uses cost of delay as its numerator.

## Connection to Queueing Theory

Cost of delay provides the economic justification for [[queueing-theory-applied]]'s prescriptions. WIP limits, [[batch-size-reduction]], and [[fast-feedback]] all reduce cycle time — but cycle time reduction only matters if there is a cost attached to delay. Cost of delay makes that cost explicit and calculable, connecting operational queueing decisions to business economics.

## Lineage

The concept draws on operations research traditions where holding cost and delay cost are standard components of inventory models. Reinertsen's contribution was applying this framing to knowledge work, where the "inventory" is unrealized features and the "holding cost" is competitive disadvantage. [[eliyahu-goldratt]]'s throughput accounting (revenue lost by not shipping) is a related but distinct framing — Goldratt focused on constraint throughput while Reinertsen focused on time-weighted opportunity cost.
