---
id: feature-driven-development
title: "Feature-Driven Development"
type: concept
importance: 5
tags:
- methodology
- fdd
- object-modeling
originator: "jeff-de-luca"
concept_type: methodology
research_status: draft
---

Feature-Driven Development (FDD) is an iterative and incremental software development methodology created by Jeff De Luca and Peter Coad around 1997 during a large banking project in Singapore. [[jon-kern]], one of the [[agile-manifesto]] signatories who co-developed FDD with De Luca, represented the FDD tradition at [[snowbird-meeting-2001]]. FDD is distinctive among pre-manifesto lightweight methods for its explicit focus on object modeling and its five-step process structure.

## The Five-Step Process

FDD organizes development around features — small, client-valued functions expressible as "action, result, object" (e.g., "calculate the total of a sale"). The five activities are:

1. **Develop an overall model** — domain modeling using object modeling techniques; done once at project start
2. **Build a feature list** — decompose the domain into subject areas, business activities, and features
3. **Plan by feature** — sequence features into development order based on dependencies and business value
4. **Design by feature** — small teams design the feature; chief programmer-led
5. **Build by feature** — implement, test, and integrate; feature sets are completed in two-week iterations

Steps 1-3 are initial (though revisited); steps 4-5 repeat per feature.

## Distinctive Characteristics

**Object modeling as foundation** — FDD is more prescriptive than other lightweight methods about how to analyze the domain. Coad's object modeling approach (Coad/Yourdon notation) provides a shared visual language for domain understanding before implementation begins. This is closer to the "firm foundations" emphasis of [[dsdm]] than to [[extreme-programming]]'s "do the simplest thing" philosophy.

**Chief programmer structure** — FDD uses small feature teams led by a chief programmer (the experienced developer who designs the feature). This differs from [[self-organizing-teams]] in that it preserves explicit technical hierarchy within feature teams while maintaining iteration and incrementality overall.

**Color-coded progress tracking** — FDD introduced "parking lot charts" showing feature completion by category and color, one of the earliest formalized [[information-radiators]] in the lightweight methods tradition.

**Scalability** — FDD was designed for larger teams (the Singapore project had over 50 people) and is more explicit about coordination mechanisms than Crystal Clear or XP, both of which were designed for small teams.

## Relationship to the Manifesto

FDD through [[jon-kern]] contributed the feature-centric view of requirements to the Snowbird conversation. The idea that requirements should be stated as features — small, deliverable, user-meaningful units of function — connects to [[user-stories]] and the Product Backlog concept. The naming is different ([[user-stories]] express who wants what and why; FDD features express what the system does), but the decomposition logic is similar.

FDD has remained a niche methodology, adopted primarily in financial services contexts where its object-modeling rigor and scalability are valued. It has not built the certification and consulting ecosystem that propelled [[scrum]] to market dominance.
