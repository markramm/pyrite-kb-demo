---
id: postmortem-practice
title: "Postmortem Practice"
type: practice
importance: 6
tags:
- organizational
- third-way
- learning
- blameless
- safety-science
practice_type: organizational
originated_in: "Safety science and aviation; adapted to IT through Etsy/Allspaw and Google SRE"
related_practices:
- incident-management
- monitoring-and-observability
status: active
research_status: draft
---

A postmortem (also called a post-incident review, or incident review) is a structured retrospective analysis conducted after a significant production incident. The DevOps and SRE postmortem practice focuses on understanding systemic causes, not assigning individual blame. The output is a document that establishes a timeline, identifies contributing factors, captures what went well and what did not, and produces concrete action items. The postmortem is the primary mechanism through which organizations learn from failure.

## Origins: Safety Science and Aviation

The practice predates software. Aviation and nuclear power developed systematic incident review processes in the mid-20th century as the industries recognized that disasters in high-reliability systems are rarely caused by single points of failure or individual incompetence. Charles Perrow's *Normal Accidents* (1984) and James Reason's Swiss Cheese model (1990) formalized the insight: complex systems fail through the conjunction of multiple contributing factors, not because one person made a mistake. Investigating *why* those factors aligned — rather than *who* failed — produces learning that prevents future incidents.

Sidney Dekker's *The Field Guide to Understanding 'Human Error'* (2006) extended this to the concept of "local rationality": people make sense of their situation with the information available to them. From the outside, post-incident, a decision looks wrong; from the inside, at the time, it was the best available option. Postmortems that ignore local rationality — that treat good-faith errors as culpable failures — will always reach wrong conclusions about causation.

## IT Adoption: Allspaw and Etsy

[[john-allspaw]] brought safety science thinking explicitly to web operations. His 2012 blog post "Blameless PostMortems and a Just Culture" (Etsy Engineering) is the founding document of the blameless postmortem movement in DevOps. Allspaw argued that engineering organizations that punish people for incidents create incentives to hide problems, not report them, and not take the kind of risks that lead to learning. The antidote is a [[blameless-postmortems]] practice: examine the system, not the individual.

Etsy's engineering culture made postmortems a routine practice for any significant incident, not just catastrophic ones. This normalized the process and removed the stigma — a postmortem is not an inquisition, it is a standard engineering artifact.

## Google SRE Formalization

[[site-reliability-engineering-book]] (Google, 2016) included a detailed chapter on postmortem culture and provided Google's postmortem template as a model. The SRE postmortem framework requires:

- **No blame**: the postmortem examines contributing factors in the system, not individual fault.
- **Timeline**: a precise chronological reconstruction of events — what was observed, when, by whom, and what actions were taken.
- **Root cause analysis**: identification of contributing factors (often multiple). The "five whys" technique, adapted from Toyota production system practice, is commonly used to trace from symptom to systemic cause.
- **Detection and response assessment**: how long did it take to detect the incident? How long to respond? What slowed the response?
- **Action items**: specific, assignable, measurable improvements — to code, infrastructure, tooling, process, or documentation — that reduce the probability or impact of similar incidents.
- **What went well**: capturing effective practices prevents the postmortem from being purely negative and generates learning about what to preserve.

The SRE book also documented Google's postmortem review culture: postmortems are shared internally, discussed in postmortem reading clubs, and used to inform engineering roadmaps. The learning is organizational, not individual.

## Connection to the Third Way

[[three-ways]] Third Way: postmortems are the primary Third Way mechanism in production operations. The Third Way demands converting individual experience into organizational learning — creating institutional memory and improving the system based on what is discovered. A postmortem document is the crystallization of that conversion: incident experience (individual) becomes documented analysis (team) becomes action items (organizational improvement) becomes reduced future risk (system improvement).

Without postmortems, the same incidents recur because the learning stays with the individuals who experienced them, and those individuals may leave, move to different teams, or simply fail to communicate what they learned. With consistent postmortem practice, the organization improves faster than individuals can.

## Psychological Safety as Prerequisite

Postmortem practice only works in organizations with sufficient psychological safety (Edmondson's concept) — where people feel safe reporting failures and uncertainties without fear of punishment. In blame cultures, postmortems become defensive exercises: participants protect themselves rather than expose systemic problems. The blameless framing is not just ethical preference; it is the technical requirement for postmortems to produce accurate information.

[[gene-kim]] and [[john-allspaw]] both point to this as a cultural precondition that tooling cannot substitute for: you can implement a postmortem template and hold scheduled reviews, but if the organizational culture is blame-oriented, the process will be performative rather than generative.

## Deming Connection

Deming's Plan-Do-Study-Act cycle and his emphasis on studying defects as system outputs rather than worker failures map directly to the postmortem discipline. Deming's claim that 94% of quality problems are system problems (not worker problems) is the statistical argument for blamelessness: if the system mostly determines outcomes, investigating the system is what improves outcomes. The postmortem is PDSA applied to production incidents: the incident is the defect; the postmortem is the study phase; the action items are the Act.

## Postmortem as Learning Artifact

High-performing organizations treat postmortems as shared intellectual property:

- Published internally (and sometimes externally — Cloudflare, GitHub, and others publish public postmortems for significant incidents)
- Indexed and searchable for future reference
- Reviewed across teams for cross-applicable lessons
- Used to calibrate priorities: a pattern of similar postmortem action items signals a systemic investment need

The external postmortem — publishing a detailed incident analysis to customers — has become an industry norm for SaaS companies, serving the dual purpose of customer transparency and public learning.
