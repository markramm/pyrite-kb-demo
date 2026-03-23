---
id: incident-management
title: "Incident Management"
type: practice
importance: 6
tags:
- reliability
- second-way
- on-call
- sre
- feedback
practice_type: reliability
originated_in: "ITIL service management; evolved in DevOps through SRE and blameless postmortem practices"
related_practices:
- postmortem-practice
- monitoring-and-observability
status: active
research_status: draft
---

Incident management is the structured process of detecting, responding to, mitigating, and learning from incidents — events where a production system is unavailable, degraded, or behaving incorrectly in a way that affects users. In the DevOps and SRE tradition, incident management is not primarily a bureaucratic process (the ITIL view) but an engineering discipline: a fast, systematic response to production failures that minimizes user impact, maintains team coordination under pressure, and feeds learning back into the system.

## ITIL vs. DevOps Approaches

The pre-DevOps approach to production incidents was shaped by ITIL (Information Technology Infrastructure Library), which treated incident management as a formal service desk process: tickets opened, priority assigned by category, escalation paths defined in advance, SLAs governing response times. ITIL incident management is designed for predictability and auditability — appropriate for the organizational context of large IT departments managing stable infrastructure.

DevOps and SRE challenged this approach from the operations side. [[john-allspaw]] and [[paul-hammond]] at Flickr — and later Etsy — demonstrated that high-frequency deployment organizations needed incident response that was fast, collaborative, and learning-focused rather than procedure-focused. The question was not "did we follow the process?" but "how quickly did we restore service and what did we learn?"

[[site-reliability-engineering-book]] (Google, 2016) formalized the SRE approach: incident management as an engineering practice with specific roles (incident commander, communications lead, operations lead), clear protocols for escalation and handoff, and a structured post-incident process (the [[postmortem-practice]]).

## Core Elements

**Detection**: incidents begin with [[monitoring-and-observability]] alerts or user reports. Detection speed is a key variable — Mean Time to Detect (MTTD) is distinct from Mean Time to Restore (MTTR) and both affect the overall blast radius of an incident. Early detection limits user impact.

**Declaration**: declaring an incident (rather than treating a problem as routine troubleshooting) triggers the structured response process. Mature incident management cultures err on the side of declaring — the cost of an unnecessary incident declaration is lower than the cost of under-responding to a real incident.

**Incident Commander**: the SRE model defines an Incident Commander (IC) — a single person responsible for coordinating the response, delegating tasks, maintaining situational awareness, and making decisions about escalation and resolution. The IC does not do technical work during the incident; their role is coordination. This role structure prevents the "too many cooks" failure mode where multiple engineers simultaneously apply conflicting mitigations.

**Communications**: keeping stakeholders informed without overloading responders. Dedicated incident channels (Slack/Teams), status pages (Statuspage, Atlassian), and structured updates at defined intervals. Communications lead handles external communication; IC handles internal coordination.

**Mitigation vs. Root Cause**: incident management distinguishes between mitigation (restoring service, even via workaround) and root cause fix. The priority during an incident is mitigation. Root cause analysis happens after service is restored, in the [[postmortem-practice]]. This distinction prevents responders from delaying recovery while pursuing elegant solutions.

**On-Call**: the human infrastructure of incident management. High-performing DevOps organizations use on-call rotations where the engineers who build the systems carry the pager — "you build it, you run it." This creates direct feedback between production behavior and development decisions. PagerDuty, OpsGenie, and VictorOps (now Splunk On-Call) are the primary tooling platforms.

## Connection to the Three Ways

[[three-ways]] Second Way: incident management is the most critical Second Way practice. The Second Way demands fast feedback from production to development; incidents are the highest-priority production feedback signal. MTTR is one of the [[dora-four-key-metrics]] — it directly measures Second Way effectiveness.

[[three-ways]] Third Way: the incident feeds into [[postmortem-practice]], which converts individual incident experience into organizational learning. Incidents are not just problems to be fixed; they are learning opportunities for the system. High-performing organizations — Etsy, Netflix, Google — institutionalized this learning cycle, treating each significant incident as an investment in organizational resilience.

## You Build It, You Run It

[[john-allspaw]] at Etsy articulated the "you build it, you run it" principle: the team that writes a service carries the pager for that service. This reverses the pre-DevOps separation between development (writes code) and operations (runs it). The consequence: developers experience directly the operational consequences of their architectural and implementation decisions. This creates the feedback loop that the DevOps model depends on — on-call experience informs code design in ways that no amount of specification or review can replicate.

The contrasting organizational model — a separate operations team that carries pagers for all production systems — severs this feedback loop. Operations accumulates knowledge about production behavior; developers remain insulated from it. [[dev-ops-cooperation]] is the concept that the "wall of confusion" between Dev and Ops is the core organizational problem DevOps addresses.

## DORA Evidence

[[accelerate-book]] and the [[state-of-devops-report-series]] identify MTTR as one of the four key metrics distinguishing high from low performers. High performers restore service significantly faster than low performers: the difference is measured in minutes and hours, not days and weeks. The practices associated with fast MTTR include [[monitoring-and-observability]] (fast detection and diagnosis), runbooks (documented response procedures), chaos engineering ([[chaos-engineering]]) to pre-test failure scenarios, and the on-call culture that ensures the right people are available and practiced.
