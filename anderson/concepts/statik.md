---
id: statik
title: "STATIK"
type: concept
importance: 7
tags:
- design-method
- systems-thinking
- onboarding
- kanban-design
- workflow-design
first_appeared: "kanban-book"
key_writings:
- kanban-book
- essential-kanban-condensed
- kanban-maturity-model
related_concepts:
- kanban-method
- visualize-workflow
- classes-of-service
- evolutionary-change
- kanban-maturity-model-concept
- make-policies-explicit
source_tradition: "systems thinking, original"
research_status: draft
---

STATIK — Systems Thinking Approach to Introducing Kanban — is a structured method for designing a kanban system tailored to a specific organizational context. It provides a principled starting point for the [[evolutionary-change]] philosophy's "start with what you do now" by ensuring that "what you do now" is analyzed rigorously before a board design is proposed.

## The Problem STATIK Addresses

A common failure mode in Kanban adoption is copying someone else's board. A team sees a compelling example — a case study from [[kanban-book]], a conference talk from the Lean Kanban conferences — and replicates the visual structure without understanding whether it fits their work type, demand profile, and capability. The result is a board that looks like a kanban system but doesn't reflect how work actually flows, and therefore doesn't surface useful information.

STATIK addresses this by insisting that board design follow analysis, not precede it.

## The STATIK Steps

The mature STATIK formulation (developed through [[lean-kanban-inc]] training programs and consolidated in teaching materials by Anderson and collaborators including [[andy-carmichael]]) typically proceeds through these analytical steps:

1. **Understand sources of dissatisfaction.** Interview stakeholders — team members, managers, customers — about what frustrates them about the current system. Dissatisfaction is data: it identifies where the pain is. This step also builds social legitimacy for the design process.

2. **Analyze demand.** Understand the volume, variety, and variability of incoming work requests. What types of work arrive? How frequently? How variable is the volume? This analysis informs decisions about [[classes-of-service]] and WIP limits.

3. **Analyze capability.** Understand the team's capacity: how many people, what skills, what constraints. Capability analysis reveals where bottlenecks are likely to form and where slack exists.

4. **Model the workflow.** Map the actual workflow — not the idealized process diagram, but the real sequence of states that work items pass through. This often reveals hidden queues, informal approval steps, and handoffs that the official process description omits.

5. **Discover classes of service.** Based on the demand analysis and stakeholder dissatisfaction data, identify the appropriate [[classes-of-service]] for this context. What urgency categories are meaningful here? What SLAs should be differentiated?

6. **Design the kanban system.** Synthesize the preceding analysis into a board design: workflow columns, WIP limits, swim lanes for classes of service, policies for each column and class.

7. **Socialize and negotiate.** Present the proposed design to stakeholders, gather feedback, and negotiate the policies (especially WIP limits and class-of-service criteria). This is not a sign-off formality but a genuine engagement with people whose cooperation the system requires.

## The Systems Thinking Foundation

The "systems thinking" in STATIK is not decorative. Anderson drew on the recognition that a kanban system is a model of a service delivery system, and models should reflect the structure and behavior of the system they represent. A board designed without analyzing demand and capability is not a model; it is a template.

The systems thinking orientation also shapes how problems are diagnosed. When items age in a column, STATIK-informed analysis asks: is this a capacity problem (not enough people)? a demand problem (too many items of this type)? a policy problem (unclear entry or exit criteria)? a skills problem (work arrives that the team cannot handle)? Each diagnosis implies a different intervention.

## STATIK in the Maturity Model

The [[kanban-maturity-model-concept]] treats STATIK-literacy as a maturity indicator. Early-stage organizations design their boards intuitively and iterate from there. More mature organizations use formal STATIK analysis when establishing new services, redesigning workflows after significant demand changes, or onboarding new teams. The formality of the analysis scales with the complexity and risk of the service context.

[[andy-carmichael]] was involved in developing and teaching STATIK as part of the [[lean-kanban-inc]] and later [[kanban-university]] curriculum.
