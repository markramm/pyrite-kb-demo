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

## Next steps

- [[connecting-via-mcp]] — connect your AI to Pyrite
- [[search-modes]] — learn how to find things
- [[understanding-entry-types]] — how knowledge is structured
- [[self-hosting]] — run your own instance
