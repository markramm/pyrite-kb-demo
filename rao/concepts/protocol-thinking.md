---
id: protocol-thinking
title: Protocol Thinking
type: concept
tags:
- protocol-design
- technology-governance
- coordination
- internet-architecture
- decentralization
links:
- target: auftragstaktik
  relation: related_to
  note: Rao's protocol thinking (shared frameworks enabling decentralized action)
    maps closely to Boyd's auftragstaktik — implicit coordination through shared doctrine
    rather than explicit orders
  kb: boyd
importance: 8
first_appeared: Breaking Smart Season 1 (2015); developed in Summer of Protocols (2023)
key_writings:
- breaking-smart-season-1
- unreasonable-sufficiency-of-protocols
- ribbonfarm-blog
- contraptions-newsletter
related_concepts:
- internet-of-beefs
- cozyweb
- blogchain
- legibility
- narrative-driven-decision-making
coined_term: false
cultural_adoption: moderate
research_status: draft
---

Protocol thinking is Venkatesh Rao's framework for understanding coordination, governance, and technology through the lens of protocols — shared rules and conventions that enable interaction without requiring central coordination. Rao develops the concept across multiple writings but most extensively in his work for the [[summer-of-protocols]] (2023), including the essay [[unreasonable-sufficiency-of-protocols]], as well as through [[breaking-smart-season-1]] (2015) and [[contraptions-newsletter]].

## The Core Concept

A protocol, in Rao's framework, is a shared set of rules that allows different parties to interact and coordinate without requiring a central authority to manage every transaction. The internet protocols (TCP/IP, HTTP) are the canonical example: they enable global connectivity without any single entity controlling the interaction. Rao generalizes from internet protocols to a broader category of social, institutional, and technical coordination mechanisms that share this structure.

Protocol thinking is the disposition to analyze coordination problems — in technology, governance, markets, and social life — by identifying the underlying protocol structure and asking what protocol design would best enable the desired coordination. It is contrasted with platform thinking (centralizing coordination in a platform that mediates all interactions) and with planning thinking (designing specific outcomes rather than enabling rules).

## The Breaking Smart Context

Protocol thinking emerges in Rao's work in the context of [[breaking-smart-season-1]], his 2015 essay series commissioned by [[andreessen-horowitz]]. The Breaking Smart thesis — that software is "eating the world" in the sense of converting industrial-era, planned, legible systems into protocol-driven, emergent, complex ones — positions protocol thinking as the fundamental orientation of the software-driven transformation. Rao argues that software's power is not in automation but in protocolization: converting activities governed by hierarchical control into activities governed by decentralized rules.

## The Summer of Protocols

Rao's most sustained development of protocol thinking came through his leadership of [[summer-of-protocols]] (2023), a research program associated with the [[ethereum-foundation]]. The program funded researchers to explore protocols across disciplines — legal, social, biological, technical — and produced [[unreasonable-sufficiency-of-protocols]], Rao's essay synthesizing the program's findings. This essay argues that protocols are remarkably sufficient as coordination mechanisms despite being dramatically under-powered compared to what we might naively expect — they accomplish enormously complex coordination with surprisingly simple rules.

## Protocol vs. Platform

A central tension in Rao's protocol thinking is the historical oscillation between protocol-dominant and platform-dominant internet eras. The early internet was protocol-dominant: HTTP, SMTP, and TCP/IP enabled global coordination without central platforms. The social media era was platform-dominant: Facebook, Google, Twitter centralized coordination in ways that allowed rapid scaling but also created the [[internet-of-beefs]] dynamics and the platform dependency that [[cozyweb]] represents a partial escape from.

Rao argues that blockchain and related decentralized technologies represent an attempt to return to protocol dominance — to enable coordination without the platform intermediary. His engagement with the [[ethereum-foundation]] reflects genuine intellectual interest in this possibility, not merely financial or professional affiliation.

## Protocol Thinking as Design Orientation

In practice, protocol thinking as a design orientation involves:

**Separation of concerns.** Protocols separate the coordination mechanism from the applications built on it. Good protocol design minimizes what the protocol specifies, leaving maximum flexibility to applications.

**Incentive alignment through structure.** Unlike platform governance (which requires enforcement of rules by a central authority), protocol governance works when the protocol's structure makes compliance the path of least resistance. Bitcoin's proof-of-work protocol is the extreme case: it is expensive to defect and profitable to comply.

**Legibility and illegibility.** Rao connects protocol thinking to his engagement with [[legibility]] — the best protocols make certain things legible (the information needed for coordination) while leaving other aspects of participants' behavior opaque and unconstrained. Over-specification kills the protocol's generativity.

## External Articulations

Rao has explained the protocol thinking framework to several adjacent intellectual communities. The [[gradient-podcast-rao]] episode (2023), recorded for The Gradient's technically sophisticated AI-adjacent audience, situates protocol thinking within the AI conversation — addressing how formal protocols interact with emergent AI behavior and what the scaling of intelligent systems does to coordination. This represents the framework's translation into the AI discourse from its origins in internet-architecture and organizational theory.

## Relationship to Narrative and OODA

Protocol thinking connects to [[narrative-driven-decision-making]] through the concept of orientation. Organizations and individuals that internalize protocol thinking have a different orientation to coordination problems than those who default to platform or planning thinking. The OODA loop operates differently when you're navigating a protocol (no central authority to appeal to, rules are emergent and evolutionary) versus a platform (rules are set by the platform operator, authority is explicit).
