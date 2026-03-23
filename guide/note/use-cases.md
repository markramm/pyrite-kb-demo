---
id: use-cases
type: note
title: "Use Cases"
tags: [overview, concepts]
importance: 7
---

Pyrite is designed to be general-purpose knowledge infrastructure. Here's how different audiences use it.

## Investigative journalism

Track people, organizations, events, claims, and evidence with source chains and reliability tiers. The journalism-investigation plugin adds:

- **Claim entries** with lifecycle management (unverified → corroborated → confirmed)
- **Evidence entries** linking claims to sources
- **Source reliability tiers** (Tier 1: direct observation, Tier 2: court records, etc.)
- **Ownership chain mapping** and money flow tracking
- **Cross-KB entity correlation** for multi-investigation searches

The knowledge graph shows connections between entities. Wikilinks create a web of evidence that's searchable by both humans and AI agents.

## Software teams

Manage architecture decisions, component documentation, backlogs, and coding standards. The software-kb plugin adds:

- **ADRs** (Architecture Decision Records) with status tracking
- **Component docs** with dependency graphs
- **Backlog items** with kanban workflow and quality gates
- **Standards** — both coding conventions and automated validation rules
- **Runbooks** for operational procedures

Works alongside your codebase — put the KB in the same repo and Claude Code can reference it while coding.

## Personal knowledge management

Build a second brain with the zettelkasten plugin:

- Notes progress through maturity stages: capture → elaborate → question → refine → connect
- Wikilinks create an organic structure that emerges from connections
- Semantic search finds conceptually related notes across your entire collection
- AI agents can help with linking, summarizing, and gap analysis

## Research and OSINT

Build structured databases of open-source intelligence:

- Typed entries enforce consistent data capture
- Source tracking with verification metadata
- Timeline views for chronological analysis
- Cross-KB search for multi-project investigations
- Git-native storage for distributed, privacy-preserving collaboration

## Team wikis and documentation

Replace Notion/Confluence with something you own:

- Markdown files work in any editor
- Git handles versioning, branching, review
- No per-seat pricing — unlimited users on self-hosted
- MCP means your team's AI tools can read the wiki
- Schema validation keeps content quality high without manual enforcement
