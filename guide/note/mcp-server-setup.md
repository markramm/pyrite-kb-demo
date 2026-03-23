---
id: mcp-server-setup
type: note
title: "MCP Server: Local and Remote Setup"
tags: [mcp, deployment, getting-started]
importance: 8
---

Pyrite's MCP server lets AI agents interact with your knowledge bases. It can run locally alongside your AI client, or serve a remote Pyrite instance.

## Local MCP server (most common)

After installing Pyrite and creating a KB:

```bash
pyrite mcp                    # write tier (default)
pyrite mcp --tier read        # read-only for untrusted agents
pyrite mcp --tier admin       # full access including reindex
```

The MCP server runs as a stdio process — your AI client (Claude, Codex, Gemini) launches it automatically via the MCP config. You don't need to start it manually.

## Access tiers

| Tier | Tools available | Use case |
|------|----------------|----------|
| **read** | search, get, list, backlinks, recent | Untrusted agents, browsing |
| **write** | All read + create, update, delete, link | Your own agents |
| **admin** | All write + reindex, schema, validate | Maintenance tasks |

## Rate limiting

The MCP server includes per-client rate limiting to prevent runaway agents:

- Read tier: 120 requests/minute
- Write tier: 60 requests/minute
- Admin tier: 30 requests/minute

## Available MCP tools

**Read tier:**
- `kb_search` — keyword, semantic, or hybrid search
- `kb_get` — read a single entry by ID
- `kb_batch_read` — read multiple entries in one call
- `kb_list_entries` — browse entries with filters
- `kb_recent` — recently changed entries
- `kb_backlinks` — find what links to an entry

**Write tier (adds):**
- `kb_create` — create a new entry
- `kb_update` — update an existing entry
- `kb_delete` — delete an entry
- `kb_link` — create a link between entries

**Admin tier (adds):**
- `kb_reindex` — rebuild the search index
- `kb_schema` — view KB schema and type definitions
- `kb_validate` — validate entries against schema

## Connecting to a remote Pyrite instance

If you're running Pyrite on a server (like the demo at demo.pyrite.wiki), the MCP server currently requires a local install pointed at the same KB data. Remote MCP over HTTP/SSE is on the roadmap.

**Current pattern for remote KBs:**
1. Clone the KB repo: `git clone <repo-url> my-remote-kb`
2. Register locally: `pyrite kb add my-remote-kb --name remote`
3. Index: `pyrite index build remote`
4. Connect via MCP as normal

Changes sync through git push/pull.
