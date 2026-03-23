---
id: infrastructure-as-code
title: "Infrastructure as Code"
type: concept
importance: 8
tags:
- infrastructure-automation
- configuration-management
- devops-practice
- mark-burgess
first_appeared: "Mark Burgess/CFEngine (1993); term popularized by Andrew Clay Shafer and the DevOps movement"
key_writings:
- continuous-delivery-book
- the-devops-handbook
related_concepts:
- deployment-pipeline
- continuous-delivery
- promise-theory
concept_type: pattern
research_status: draft
---

Infrastructure as Code (IaC) is the practice of managing and provisioning computing infrastructure through machine-readable definition files — version-controlled, tested, and deployed using the same practices applied to application code — rather than through manual processes or ad-hoc configuration. It is a foundational enabler of [[continuous-delivery]] and the [[deployment-pipeline]], extending automated delivery past the application layer into the systems that run applications.

## Definition

The core principle: infrastructure state is expressed as code (or configuration), committed to version control, and applied to systems by an automated agent. The desired end state is declared; the tooling handles the execution path to reach it. When the code is correct, the infrastructure is reproducible, auditable, and testable.

Contrast with the manual operations baseline it replaced: servers configured by hand, SSH sessions executed by individual operators, state that existed only in operator memory or tribal knowledge. This baseline is the operational equivalent of code that is never committed to version control — functional until the person with the knowledge leaves.

## Historical Evolution

The lineage spans three decades:

**CFEngine (1993)**: [[mark-burgess]] created CFEngine at Oslo University — the first infrastructure automation tool and the first declarative configuration management system. CFEngine expressed desired system state rather than imperative commands; nodes would converge to the declared state. This was conceptually revolutionary in 1993 and established the declarative paradigm that all subsequent tools inherited. Burgess held the first academic position in Network and System Administration; CFEngine was simultaneously a research project and a practical tool.

**Puppet (2005)**: [[andrew-clay-shafer]] and Luke Kanies founded Puppet ([[puppet-labs]]) building on CFEngine's declarative model with a more accessible Ruby-based DSL. Puppet became the primary configuration management tool of the early DevOps movement and was one of the tools that made the Agile infrastructure argument credible at scale.

**Chef (2009)**: Adam Jacob's Chef offered a more code-centric approach (Ruby, not a DSL), appealing to developers who wanted full programming language expressiveness in infrastructure configuration.

**Ansible (2012, approximate)**: Michael DeHaan's Ansible offered agentless execution (SSH-based) and YAML configuration, lowering the barrier to entry and becoming dominant in the late DevOps era.

**Terraform (2014, approximate)**: HashiCorp's Terraform introduced IaC for cloud resource provisioning — not just configuration management of running systems, but the creation and lifecycle management of infrastructure itself (VMs, networks, databases, DNS). Terraform's provider model made it cloud-agnostic and became the dominant tool for cloud infrastructure management.

## Declarative vs. Imperative

IaC tools span two paradigms:

**Declarative**: You describe the desired end state; the tool determines how to reach it. CFEngine, Puppet, Terraform, and Ansible (in its idempotent mode) are declarative. The advantage: idempotency — running the same configuration twice produces the same result regardless of the starting state.

**Imperative**: You describe the sequence of steps to execute. Shell scripts and some Ansible playbooks are imperative. The advantage: precision control. The disadvantage: scripts drift from reality as systems change, and applying them multiple times can produce unintended results.

The declarative approach is generally preferred for IaC because it enables safe re-application — you can run your configuration continuously and always converge to the known-good state.

## Connection to Promise Theory

[[mark-burgess]]'s [[promise-theory]] (proposed 2004-2005 at the DISO conference, approximate) provides a formal theoretical foundation for why declarative configuration management works. Promise Theory models distributed systems as collections of autonomous agents that make promises to each other about their state, rather than receiving central commands.

Applied to IaC: a managed node "promises" to converge to the desired state described in its configuration. The configuration management server does not command the node; the node consults the declared state and self-converges. This autonomous, voluntary model is more resilient than command-and-control in distributed systems — nodes can converge even when the management server is temporarily unavailable.

Promise Theory explains why declarative IaC scales better than imperative approaches: coordination is distributed and local rather than centralized.

## Why It Matters

IaC addresses several failure modes that plagued pre-DevOps operations:

**Reproducibility**: Infrastructure defined as code can be recreated from scratch on demand — for disaster recovery, scaling events, or simply to create a test environment that matches production. Without IaC, "works in production but not in staging" is a chronic failure mode.

**Version control and auditability**: Infrastructure changes tracked in git provide a complete audit trail — what changed, when, who changed it, and why (via commit messages). This is critical for compliance, for debugging, and for enabling rollback.

**Testing**: Infrastructure code can be tested — unit tests validate that templates render correctly; integration tests validate that provisioned infrastructure behaves as expected. Testing infrastructure was essentially impossible in the manual-configuration era.

**Collaboration**: Infrastructure defined as code can be reviewed, discussed, and merged using standard developer workflows. This is the technical basis for breaking down the Dev/Ops wall — when both groups work in the same version control system with the same tooling, the organizational separation becomes harder to justify.

## Connection to the First Way

IaC is a prerequisite for extending the First Way ([[three-ways]]) past the application code boundary. A [[deployment-pipeline]] that automates application build and test but requires manual infrastructure provisioning has a manual step that creates a constraint — exactly the kind of bottleneck that lean and Goldratt's TOC ([[the-goal-for-it]]) identify as the system constraint. IaC removes that constraint, enabling the pipeline to encompass the full value stream.

[[the-devops-handbook]] explicitly extends the pipeline to include infrastructure: application code and infrastructure code go through the same pipeline, are tested together, and are deployed together. This is the definition of DevOps as a practice rather than an organizational structure.

## "Cattle Not Pets"

The "cattle not pets" metaphor — attributed to various sources in the DevOps community, popularized around 2012-2013 (approximate) — captures the cultural shift IaC enables: servers are not individually named and lovingly maintained (pets); they are fungible instances created and destroyed on demand (cattle). IaC makes this possible: if any server can be recreated from its definition, there is no operational cost to destroying and recreating it. This shift underpins cloud-native deployment patterns including [[blue-green-deployments]], [[canary-releases]], and auto-scaling.
