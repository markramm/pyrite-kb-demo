---
id: site-reliability-engineering
title: "Site Reliability Engineering (SRE)"
type: concept
importance: 8
tags:
- reliability
- operations
- google
- slo
- error-budget
- toil
concept_type: practice-category
first_appeared: "Google (coined by Ben Treynor Sloss, c. 2003); codified in SRE book (2016)"
key_writings:
- site-reliability-engineering-book
related_concepts:
- blameless-postmortems
- monitoring-and-observability
- incident-management
- dora-four-key-metrics
research_status: draft
---

Site Reliability Engineering is what happens when you ask a software engineer to design an operations function. That definition, from Ben Treynor Sloss at Google, is more than a quip — it describes the founding logic: treat operations problems as software problems, and bring software engineering discipline (measurement, automation, systematic analysis) to bear on keeping systems running at scale.

Google created the SRE role around 2003, internally. It remained a Google-specific practice for over a decade before the 2016 [[site-reliability-engineering-book]] made the principles available to the broader industry.

## Error Budgets and the Mathematics of Failure

The central SRE innovation is the error budget. An SLO (Service Level Objective) defines the reliability target — say, 99.9% uptime. The remaining 0.1% is the error budget: the permissible amount of unreliability that can be "spent" on product changes, experiments, and risk-taking.

This reframes the perennial dev-ops conflict. Operations wants stability; development wants to ship features. The error budget converts that argument into a negotiated quantity. If the budget is intact, deploy freely. If the budget is exhausted, slow down until reliability recovers. Both sides agree to the math in advance.

The SLO concept draws from control theory and process engineering — reliability targets that define acceptable operating ranges rather than aspirational maximums.

## Toil Reduction

SRE practice formally defines "toil" as manual, repetitive, automatable work that scales linearly with service growth. SRE teams target toil reduction as a primary engineering activity. The goal is to maintain toil below 50% of an SRE's time, with the remainder spent on engineering work that reduces future toil.

This is lean waste elimination (muda) applied to operations work — identifying and systematically eliminating repetitive manual effort. The connection to the [[three-ways]] is direct: toil is a form of waste that degrades flow.

## SRE and DevOps

Google's own framing: "SRE is what you get if you implement DevOps." [[three-ways]] is the philosophy; SRE is one implementation. DevOps describes principles — flow, feedback, learning. SRE provides a specific organizational model and a specific set of practices for implementing those principles in an engineering context.

The distinctions matter. SRE uses job titles (Site Reliability Engineer), formal staffing ratios, error budgets as governance mechanisms, and embedded reliability teams. DevOps as described in [[the-devops-handbook]] is more agnostic about org structure. Both converge on shared ownership of reliability between dev and ops.

Connection to the [[three-ways]]:
- **First Way (Flow)**: toil reduction and automation eliminate bottlenecks in production systems
- **Second Way (Feedback)**: SLOs and SLIs create fast, measurable feedback about system health
- **Third Way (Learning)**: [[blameless-postmortems]] are a formal SRE mechanism for organizational learning from incidents

## The Google Provenance Problem

SRE originated at Google and reflects Google's specific context: scale (billions of users), engineering culture (hire PhDs, expect deep systems knowledge), and resources (budget for dedicated reliability teams). Many SRE practices presuppose a level of engineering sophistication and staffing that most organizations cannot match.

This is a legitimate limitation. The error budget model requires mature SLO definition. Embedded SRE teams require a certain organizational scale to justify. The [[site-reliability-engineering-book]] is largely descriptive of how Google operates, not prescriptive for general adoption. The 2018 "SRE Workbook" attempted to address generalizability, with mixed results.

## Relationship to DORA Research

The [[dora-four-key-metrics]] — especially Time to Restore Service and Change Failure Rate — map directly onto SRE concerns. [[accelerate-book]] provides empirical evidence that the practices SRE prescribes (monitoring, incident management, blameless postmortems) correlate with higher software delivery performance and organizational outcomes. This gives SRE a research foundation that the original Google book, being largely case-study based, lacked.
