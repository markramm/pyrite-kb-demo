---
id: what-is-pyrite
type: note
title: "What is Pyrite?"
tags: [overview, getting-started]
importance: 10
---

Pyrite is a knowledge infrastructure platform. You store structured knowledge in markdown files with YAML frontmatter, validated against schemas, versioned in git, and searchable by any AI through MCP.

## The problem Pyrite solves

Your AI agents have no memory. Your knowledge is trapped in platform silos. Every new chat starts from zero. Pyrite gives you structured, validated, git-versioned knowledge bases that any AI can read and write through a built-in MCP server.

## How it works

1. **Markdown files are the source of truth** — plain text with YAML frontmatter, readable in any editor
2. **A search index** (SQLite FTS5 + optional vector embeddings) sits on top for fast search
3. **Multiple interfaces** access the same data: CLI, REST API, MCP server, and this web UI
4. **Plugins** add domain-specific entry types, tools, and workflows

## What makes Pyrite different

- **Typed entries with schema validation** — not flat vector blobs. Define person, organization, event, concept types with validated fields.
- **Git-native** — every change is a versioned commit. Branch, diff, review, rollback.
- **MCP server with three-tier access control** — read/write/admin tiers for AI agents.
- **Semantic + structured search** — find by meaning (vector embeddings) AND by type, tag, date range, or relationship.
- **Plugin system** — custom entry types, MCP tools, CLI commands, validators, lifecycle hooks.
- **Zero running cost locally** — markdown files + SQLite on your disk. No cloud dependency.

## Get started

- [[local-install]] — install Pyrite on your machine
- [[getting-started]] — create a KB and add entries
- [[connecting-via-mcp]] — connect your AI to Pyrite

## Use with AI

- [[using-with-claude-code]] — Pyrite as a knowledge layer for Claude Code
- [[using-with-claude-desktop]] — persistent memory for Claude Desktop and Cowork
- [[mcp-server-setup]] — MCP server tiers, tools, and remote access
- [[ai-features-and-api-keys]] — configure AI for summarize, auto-tag, and chat

## The platform

- [[web-ui-features]] — dashboard, entries, graph, editor, keyboard shortcuts
- [[understanding-entry-types]] — how knowledge is structured
- [[search-modes]] — keyword, semantic, and hybrid search
- [[knowledge-graph]] — connections and backlinks
- [[plugins-and-extensions]] — extend Pyrite for your domain

## Deeper

- [[design-principles]] — architecture and design philosophy
- [[vision-and-roadmap]] — where Pyrite is headed
- [[use-cases]] — journalism, software teams, research, PKM
- [[self-hosting]] — run your own instance
- [[for-developers]] — CLI, REST API, MCP, Python API
