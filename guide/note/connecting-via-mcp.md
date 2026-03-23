---
id: connecting-via-mcp
type: note
title: "Connecting Your AI via MCP"
tags: [mcp, getting-started, claude, openai, gemini]
importance: 10
---

Pyrite includes a built-in MCP (Model Context Protocol) server. Any AI that speaks MCP can search, read, and write your knowledge bases.

## Claude Desktop or Claude Code

Add this to your MCP configuration:

```json
{
  "mcpServers": {
    "pyrite": {
      "command": "pyrite",
      "args": ["mcp"]
    }
  }
}
```

**Claude Desktop:** Edit `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) or `%APPDATA%\Claude\claude_desktop_config.json` (Windows).

**Claude Code:** The config is at `~/.claude/claude_code_config.json`, or add it through Settings.

After restarting, Claude can search your KBs, read entries, create new ones, and follow wikilinks — all through natural conversation.

## OpenAI Codex CLI

Add to `~/.codex/config.toml`:

```toml
[mcp.servers.pyrite]
command = "pyrite"
args = ["mcp"]
```

## Gemini CLI

Add to `~/.gemini/settings.json`:

```json
{
  "mcpServers": {
    "pyrite": {
      "command": "pyrite",
      "args": ["mcp"]
    }
  }
}
```

## What the MCP server provides

Pyrite exposes three tiers of MCP tools:

- **Read tier** (default): `kb_search`, `kb_get`, `kb_list_entries`, `kb_batch_read`, `kb_recent`, `kb_backlinks`
- **Write tier**: `kb_create`, `kb_update`, `kb_delete`, `kb_link`
- **Admin tier**: `kb_reindex`, `kb_schema`, `kb_validate`

Start the MCP server with a specific tier:

```bash
pyrite mcp                    # write tier (default)
pyrite mcp --tier read        # read-only for untrusted agents
pyrite mcp --tier admin       # full access including reindex
```

## MCP with a remote Pyrite server

If you're running Pyrite on a server (like this demo), MCP currently works with a local install pointed at the same data. Remote MCP over HTTP is on the roadmap.

For now, the recommended pattern is: install Pyrite locally, clone the KB repo, and connect via MCP locally. The web UI provides the remote browsing experience.
