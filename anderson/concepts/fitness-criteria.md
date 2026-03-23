---
id: fitness-criteria
title: "Fitness Criteria"
type: concept
tags:
- fit-for-purpose
- service-design
- customer-outcomes
- metrics
- lead-time
links:
- target: batch-size-reduction
  relation: related_to
  note: Fitness criteria (lead time, throughput) improve with smaller batch sizes — Reinertsen's batch size economics provides the theoretical foundation
  kb: reinertsen
metadata:
  first_appeared: "fit-for-purpose"
  key_writings: &id001
  - fit-for-purpose
  - kanban-maturity-model
  related_concepts: &id002
  - kanban-method
  - manage-flow
  - classes-of-service
  - implement-feedback-loops
  - kanban-maturity-model-concept
  source_tradition: "original (Fit for Purpose framework)"
  research_status: draft
first_appeared: "fit-for-purpose"
key_writings: *id001
related_concepts: *id002
source_tradition: "original (Fit for Purpose framework)"
research_status: draft
---

Fitness criteria are the metrics by which a service is evaluated as "fit for purpose" for a particular customer segment — the specific, measurable outcomes that a service must achieve to satisfy the customers who use it. The concept was developed in Anderson's *Fit for Purpose* framework, co-developed with Alexei Zheglov and published in [[fit-for-purpose]].

## The Fit for Purpose Framework

The *Fit for Purpose* framework addresses a problem that the [[kanban-method]]'s earlier formulations left partially unresolved: the method provides practices for improving flow, but what is the right level of performance to target? WIP limits and lead time management improve the system — but improve it toward what?

The Fit for Purpose answer: a service is fit for purpose when it meets the fitness criteria of the customers who depend on it. Fitness is customer-defined, not internally defined. A team that is proud of its 5-day lead time may be fit for purpose for customers who need 10-day delivery, and catastrophically unfit for customers who need 2-day delivery.

## Fitness Criteria Dimensions

Fitness criteria typically include:

- **Lead time** — does the service deliver within the time horizon customers need?
- **Throughput** — does the service produce at the volume customers require?
- **Quality** — does the service deliver defect rates within customer tolerance?
- **Predictability** — does the service deliver at consistent lead times, or is variability itself a fitness problem?
- **Safety** — (for relevant service types) does the service meet safety requirements?
- **Other context-specific measures** — customer satisfaction scores, SLA compliance rates, etc.

The key insight is that fitness criteria are context-specific and customer-segment-specific. A single service may be fit for purpose for some customer segments and not others.

## Customer Segmentation

The framework introduces explicit **customer segmentation** as a precondition for fitness analysis. Different customers have different fitness criteria. A customer who accepts 30-day lead times for non-urgent work has different needs than one who requires 24-hour response. The [[classes-of-service]] concept addresses this at the workflow policy level; fitness criteria address it at the service design level.

Zheglov's contribution was particularly significant in developing the customer segmentation analysis: understanding which customers the service is designed to serve, what their specific fitness criteria are, and whether the service is meeting them.

## Relationship to Flow Management

[[manage-flow]] provides the operational mechanism for achieving fitness criteria. Once fitness criteria are defined (e.g., "95% of Standard class items delivered within 10 days"), flow management practices — [[wip-limits]], queue management, [[implement-feedback-loops]] — can be calibrated to achieve them. The fitness criteria turn abstract flow improvement into a concrete target.

This connection makes fitness criteria the customer-facing complement to the Kanban Method's internal-facing practices. The method tells you how to manage your system; the Fit for Purpose framework tells you what outcomes you're managing it toward.

## Fitness Criteria in the Maturity Model

The [[kanban-maturity-model-concept]] places explicit fitness criteria definition at higher maturity levels (ML3-ML4). Early-stage organizations improve flow without a precise definition of what "good" means from the customer's perspective. More mature organizations have defined fitness criteria per service, track them in the Service Delivery Review feedback loop, and adjust their service design when criteria are not being met.

This developmental picture is consistent with the [[evolutionary-change]] philosophy: you don't need to define perfect fitness criteria before you start. You start with [[visualize-workflow]] and [[wip-limits]], learn what your system actually produces, and over time develop increasingly precise understanding of what your customers need.
