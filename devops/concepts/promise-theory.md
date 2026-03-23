---
id: promise-theory
title: "Promise Theory"
type: concept
importance: 5
tags:
- theory
- distributed-systems
- mark-burgess
- cfengine
- autonomy
- desired-state
concept_type: framework
first_appeared: "Mark Burgess (2004-2005); refined with Jan Bergstra"
related_concepts:
- infrastructure-as-code
research_status: draft
---

Promise theory is a formal model of distributed cooperation in which autonomous agents make promises about their own behavior, rather than being commanded by a central authority. It provides the theoretical foundation beneath practical infrastructure-as-code tools — the reason "desired state" configuration management works, stated as a first principle.

## Origin

[[mark-burgess]] developed promise theory between 2004 and 2005, initially in the context of CFEngine — his configuration management system for Unix systems administration. CFEngine was already operating on something like promise-based logic before the theory was articulated: each node independently applied configuration to achieve a specified state, rather than executing commands sent from a central server. Burgess formalized this operational reality into a theoretical framework, later refining it with mathematician Jan Bergstra.

The foundational papers appeared in the mid-2000s in systems administration and theoretical computer science contexts. The ideas gained broader circulation when Burgess published "In Search of Certainty" (2013) and "Thinking in Promises" (2015), making the theory accessible to practitioners.

## The Core Distinction: Obligation vs. Promise

Classical distributed systems thinking assumes obligation-based coordination: a central authority issues commands, and nodes execute them. This is the client-server model taken to its logical conclusion. It has a fundamental scaling problem: as the network grows and nodes multiply, the central authority becomes a bottleneck. More critically, obligation-based models require the commanding party to have accurate knowledge of the state of the commanded party — knowledge that becomes increasingly unreliable at scale.

Promise theory proposes an alternative: agents make promises about their own behavior. A node promises to maintain a certain configuration. A service promises to respond within a certain latency bound. The promise is about the agent's own outputs, not about what others will do. No central authority need verify compliance in real time; agents self-certify. Trust is built from accumulated promise-keeping, not from authority.

## Connection to Infrastructure as Code

The [[infrastructure-as-code]] paradigm — Puppet, Chef, Ansible, Terraform — operationalizes promise theory at the level of tooling. When Puppet specifies that a package should be installed and running, it is stating a promise about the node's desired state. The agent on each node reads this specification and independently works to fulfill the promise. The central authority (the Puppet master) stores and distributes the specifications but does not execute them. Each node executes its own convergence.

This is why desired-state configuration management is more robust than imperative configuration scripts. Imperative scripts say "run these commands." Promise-based systems say "achieve this state." If the state is already achieved, nothing happens. If the node drifts, the agent corrects it. The system is self-healing in a way that command execution is not.

## Cattle, Not Pets

Promise theory provides the theoretical underpinning for the "cattle not pets" operational philosophy. If each node in a cluster promises to maintain a specific state, and the tooling ensures that promise is kept, then individual nodes are fungible — interchangeable. A node that fails is simply replaced with a new instance that will make and keep the same promise. The node's individual identity is irrelevant; its promised behavior is what matters.

This connects to cloud-native infrastructure design: auto-scaling groups, immutable infrastructure, container orchestration. All presuppose that individual instances are replaceable because their behavior is specified as a promise, not embedded as unique configuration.

## Organizational Echoes

Promise theory's distributed, autonomous model has organizational parallels in the DevOps movement. The [[dev-ops-cooperation]] culture DevOps advocates — teams owning their own services, "you build it, you run it," decentralized decision-making — mirrors the promise-based model at the team level. Teams make promises about service behavior (SLOs, reliability targets, API contracts) rather than receiving commands from a central operations function. The [[cams-framework]]'s sharing pillar includes this concept of autonomous teams coordinating through agreements.

The analogy is not perfect — human organizations are not distributed computational agents — but the structural insight transfers: decentralized systems coordinated through explicit promises scale better than centralized systems coordinated through commands.
