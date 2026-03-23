---
id: economic-framework-for-prioritization
title: Economic Framework for Prioritization
type: concept
tags:
- economics
- prioritization
- decision-making
- trade-offs
- framework
links:
- target: five-focusing-steps
  relation: related_to
  note: Reinertsen's economic prioritization framework and Goldratt's five focusing
    steps both address sequencing work through a constrained system to maximize throughput
  kb: goldratt
importance: 9
first_appeared: managing-the-design-factory
key_writings:
- managing-the-design-factory
- principles-of-product-development-flow
related_concepts:
- cost-of-delay
- u-curve-optimization
- weighted-shortest-job-first
- decentralized-control
- managing-variability
research_status: draft
---

The economic framework for prioritization is Reinertsen's overarching argument: every significant product development decision is an economic trade-off, and it should be made by analyzing costs and benefits, not by applying proxy metrics, process dogma, or received wisdom. This framework is the intellectual foundation of his entire body of work — all other concepts are applications of it to specific decision domains.

## The Central Critique

Product development organizations commonly make decisions using proxy metrics — schedule adherence, test coverage percentages, sprint velocity, resource utilization. Reinertsen's argument is that proxy metrics are dangerous because they optimize for the proxy rather than the underlying economic objective. A team that maximizes resource utilization (a common proxy for efficiency) will, by [[queueing-theory-applied]], accumulate queues that impose large [[cost-of-delay]]. The proxy metric looks good; the economic outcome is bad.

Similarly, process frameworks that prescribe fixed practices (always do X, never do Y) are applying rules derived from specific economic contexts to organizations with different cost structures. The correct approach is to analyze the actual costs and benefits in each context and derive the appropriate practice from that analysis.

## The Chapter E Framework

[[principles-of-product-development-flow]] opens with a chapter on economics (Chapter E, yielding principle numbers E1-E7) that establishes the framework before introducing any operational prescriptions. The logical sequence:

1. All product development decisions have economic consequences
2. To make good decisions, you need to quantify those consequences
3. The primary economic variable is [[cost-of-delay]] — the cost per unit time of not delivering
4. Decisions should be made by trading off cost of delay against effort, quality, and risk costs
5. This framework, applied consistently, produces [[weighted-shortest-job-first]] for scheduling, [[u-curve-optimization]] for parameter choices, and [[decentralized-control]] for organizational design

## Trade-off Analysis, Not Rules

The economic framework insists on trade-off analysis rather than rules. For any practice, the question is not "is this practice good?" but "what does this practice cost and what does it produce, in this context?" The answer will vary by organization, market position, technology, and team capability. This is why Reinertsen's prescriptions are expressed as economic principles rather than process rules — the principles tell you how to analyze the decision; they do not pre-decide it.

This distinguishes Reinertsen from both traditional stage-gate processes (which prescribe specific reviews and artifacts) and from lean/agile frameworks (which prescribe specific ceremonies and practices). Both assume that the correct practice is context-independent. Reinertsen's economic framework assumes context-dependence and provides the tools for context-specific analysis.

## Making Invisible Costs Visible

A recurring theme is that delay costs are invisible while effort costs are visible. Budgets track engineering hours; they do not track the revenue lost by shipping two months late. Schedules track milestone dates; they do not track the compounding competitive disadvantage of missing a market window. The economic framework's first practical task is making these invisible costs visible — quantifying them, putting them in the same units as effort costs, and requiring that decisions account for them.

## Downstream Applications

Every other major concept in Reinertsen's framework is an application of economic analysis to a specific domain:
- [[cost-of-delay]]: quantifying the most important invisible cost
- [[weighted-shortest-job-first]]: economically optimal sequencing given delay costs
- [[u-curve-optimization]]: the structural form of trade-off analysis applied to parameters
- [[batch-size-reduction]]: economic analysis of transaction cost vs. holding cost
- [[managing-variability]]: economic analysis of variability's costs and benefits
- [[decentralized-control]]: economic analysis of decision-making structure
