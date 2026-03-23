---
id: lean-transmission-chain
title: "The Lean Transmission Chain: Ohno/Shingo → Womack/Jones → Poppendiecks → Ries"
type: note
importance: 8
tags:
- transmission-chain
- tps
- lean-software
- lean-startup
- translation
research_status: draft
---

The intellectual transmission of lean thinking from Toyota's shop floor to Silicon Valley's startups is a multi-stage translation chain. Each stage gains portability and loses specificity. [[james-p-womack]] and [[daniel-t-jones]] occupy the critical second position — they are the translators who made the chain possible.

## The Chain

### Stage 1: TPS Practitioners (1950s-1980s)
**[[taiichi-ohno]]** and **[[shigeo-shingo]]** developed the Toyota Production System through decades of shop-floor experimentation at [[toyota-motor-corporation]]. Their innovations — just-in-time, jidoka, kanban, SMED, poka-yoke — were empirical solutions to specific manufacturing problems. Ohno wrote *Toyota Production System: Beyond Large-Scale Production* (1978/1988 English translation); Shingo wrote *A Study of the Toyota Production System* (1981/1989 English). These were practitioner accounts for practitioners.

**Domain:** automotive manufacturing
**Audience:** Toyota employees and close affiliates
**Form:** operational practices, internal training, practitioner memoirs

### Stage 2: Lean Researchers (1985-2005)
**[[james-p-womack]]**, **[[daniel-t-jones]]**, and **[[daniel-roos]]** studied TPS through the [[mit-imvp]] and translated it for Western audiences. [[john-krafcik]] coined the name "lean production." [[machine-that-changed-the-world]] (1990) proved TPS was superior empirically. [[lean-thinking]] (1996) codified the [[five-lean-principles]]. The [[lean-enterprise-institute]] and [[lean-enterprise-academy]] institutionalized the transmission.

**Domain:** general management
**Audience:** Western executives and managers
**Form:** research-based books, HBR articles, frameworks, institutions

**What changed in this stage:** TPS practices were abstracted into principles. The system's cultural embeddedness was stripped away. The framework became portable but lost operational specificity. See [[tps-to-lean-translation]].

### Stage 3: Lean Software Development (2003-2010)
Mary and Tom Poppendieck translated Lean principles into software development in *Lean Software Development* (2003) and *Implementing Lean Software Development* (2006). They mapped the [[five-lean-principles]] to software concepts: eliminating waste (unnecessary code, extra features), building quality in, creating knowledge, deferring commitment, delivering fast, respecting people, and optimizing the whole.

**Domain:** software development
**Audience:** software engineers, team leads, agile practitioners
**Form:** books, conference talks, consulting

**What changed in this stage:** Manufacturing metaphors became knowledge-work metaphors. "Inventory" became "partially done work." "Defects" became "bugs." "Batch size" became "release frequency." The Poppendiecks explicitly acknowledged Womack and Jones as their source, maintaining the genealogical connection.

### Stage 4: Lean Startup (2008-present)
Eric Ries created the Lean Startup methodology, drawing on lean vocabulary (waste elimination, validated learning as a form of pull) and Steve Blank's Customer Development. The connection to Womack/Jones is genealogical rather than direct: Ries cites the lean tradition but builds primarily on the Poppendiecks' software translation and on Blank's entrepreneurship framework.

**Domain:** technology startups, entrepreneurship
**Audience:** founders, venture capitalists, corporate innovators
**Form:** books, blogs, accelerator programs, university courses

**What changed in this stage:** "Lean" became primarily associated with experimentation and iteration rather than with waste elimination and flow. The Build-Measure-Learn loop is structurally different from the five lean principles, though it draws on the same conceptual ancestry. The connection to TPS is now several translations removed.

## The Compounding Abstraction Problem

Each stage in the chain abstracts further from the original:
- Ohno → Womack/Jones: factory practices → management principles
- Womack/Jones → Poppendiecks: management principles → software practices
- Poppendiecks → Ries: software practices → startup methodology

By Stage 4, the connection to [[taiichi-ohno]]'s kanban system is genealogical rather than operational. A startup founder running Build-Measure-Learn sprints has almost no operational overlap with a Toyota production line — but the intellectual ancestry is traceable.

This compounding abstraction is not unique to lean. It is the normal process by which operational innovations become management philosophies become cultural vocabulary. But it means that "lean" in a 2025 startup context means something very different from "lean" in Womack and Jones's 1996 context, which in turn means something different from what Ohno practiced on Toyota's shop floor.

## Womack and Jones's Position

Womack and Jones are the bottleneck in this chain — the point through which all downstream translations must pass. Without [[machine-that-changed-the-world]], the Western world does not have a vocabulary for TPS. Without [[lean-thinking]], there are no five principles to translate to software or startups. Without the [[lean-enterprise-institute]], there is no institutional infrastructure for spreading lean ideas.

Their position is powerful but also limiting. The downstream translations inherit both the insights and the blind spots of Womack and Jones's codification. The underemphasis on "respect for people" in the five principles propagates to lean software and lean startup, where people concerns are often secondary to process optimization. The sequential framing of the principles propagates as well — creating the impression that lean is a step-by-step methodology rather than an interlocking system.

## Research Needed

- Whether the Poppendiecks had direct contact with Womack/Jones or worked primarily from their publications
- Whether Ries explicitly cites Womack/Jones or arrives at "lean" through the Poppendiecks
- Other transmission chains not covered here: lean in healthcare, lean in government, lean in construction
