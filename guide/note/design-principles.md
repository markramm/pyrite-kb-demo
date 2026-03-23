---
id: design-principles
type: note
title: "Design Principles and Architecture"
tags: [architecture, concepts, design]
importance: 8
---

Pyrite's design reflects specific beliefs about how knowledge infrastructure should work. These principles inform every architectural decision.

## Core principles

### Files are the source of truth

Every entry is a markdown file with YAML frontmatter. The SQLite index is derived — delete it and rebuild from files with `pyrite index build`. This means:

- Your data is never locked in a database
- You can edit entries in any text editor
- Git tracks every change with full history
- Moving to another tool means copying files

### Git-native, not git-compatible

Pyrite doesn't just support git — it assumes git. Every KB is a git repository. Changes are commits. Collaboration is branches and merges. This gives you:

- Full audit trail for every change
- Branch for experiments, merge when ready
- Standard code review workflows for knowledge
- Signed commits for attestation (who wrote what, when)

### Schema validates, not constrains

Type schemas in `kb.yaml` define what fields an entry SHOULD have, not what it CAN have. Validation warns about missing required fields but doesn't prevent creation. This keeps the system usable while maintaining data quality over time.

### AI is optional and BYOK

Every feature works without AI. Semantic search uses a local model. Summarize, auto-tag, and chat require an API key — but only if you want them. No telemetry, no cloud dependency, no surprise API calls.

### MCP-first agent interface

The MCP server is a first-class interface, not an afterthought. AI agents get the same data model, access controls, and search capabilities as human users. Three tiers (read/write/admin) let you give different agents different trust levels.

## Architecture

```
Markdown files (source of truth)
    ↓ index build
SQLite FTS5 + sqlite-vec (search index)
    ↓ accessed by
┌─────────────┬──────────────┬───────────────┬──────────────┐
│    CLI      │  REST API    │  MCP Server   │   Web UI     │
│  (pyrite)   │ (pyrite-svr) │ (pyrite mcp)  │  (SvelteKit) │
└─────────────┴──────────────┴───────────────┴──────────────┘
```

### Storage layer

- **Markdown files**: YAML frontmatter + body. One file per entry, organized by type subdirectory.
- **SQLite FTS5**: Full-text search index with BM25 ranking.
- **sqlite-vec**: Vector embeddings for semantic search (optional).
- **PostgresBackend**: Alternative for server deployments (tsvector + pgvector).

### Service layer

Business logic is in focused services, not monolithic classes:

- **KBService**: Entry CRUD, indexing hooks
- **SearchService**: Keyword, semantic, hybrid search with RRF
- **GraphService**: Link queries, backlinks, graph data
- **EmbeddingService**: Vector storage and similarity search
- **ExportService**: KB export to directories or git repos

### Plugin system

Plugins are Python packages using entry points. The protocol defines 15 methods covering:

- Entry types and field schemas
- MCP tools (per tier)
- CLI commands
- Validators and quality checks
- Relationship types
- Init templates
- Lifecycle hooks (before/after save)

### Two-tier durability

- **Tier 1 (git)**: Entry content, KB configuration, schemas — everything that matters
- **Tier 2 (SQLite)**: Search index, embeddings, engagement data — derived and rebuildable

If you lose the SQLite database, rebuild it from files. If you lose the files, you've lost data.
