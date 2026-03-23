---
id: using-with-claude-code
type: note
title: "Using Pyrite with Claude Code"
tags: [claude, mcp, getting-started, agent]
importance: 9
---

Claude Code is Anthropic's CLI agent for software development. When connected to Pyrite via MCP, Claude Code can search, read, and write your knowledge bases as part of its workflow.

## Setup

1. Install Pyrite locally: `pip install "pyrite[all]"`
2. Create or clone a KB (see [[local-install]])
3. Add Pyrite to your Claude Code MCP config

### Claude Code MCP configuration

Edit `~/.claude/claude_code_config.json` (or add via Claude Code settings):

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

Restart Claude Code. Pyrite's MCP tools are now available.

## What Claude Code can do with Pyrite

- **Search your KB**: "What do we know about authentication patterns?"
- **Read entries**: "Show me the ADR for our database choice"
- **Create entries**: "Create a component doc for the new auth service"
- **Follow links**: "What's connected to the rate limiter component?"
- **Manage backlogs**: "What's the status of the export feature?"

## Example workflow

You're working on a codebase that has a Pyrite KB (like Pyrite itself):

```
You: "Search the KB for how the plugin system works"
Claude: [uses kb_search to find plugin-related entries]
Claude: "Based on the component docs, the plugin system uses..."

You: "Create a backlog item for the new feature we discussed"
Claude: [uses kb_create to create a backlog_item entry]
```

## Access tiers

By default, Claude Code gets **write** tier access. For read-only:

```json
{
  "mcpServers": {
    "pyrite": {
      "command": "pyrite",
      "args": ["mcp", "--tier", "read"]
    }
  }
}
```

## Tips

- Put your KB in the same repo as your code — Claude Code sees both
- Use the `software` template for software projects: `pyrite init --template software --path kb`
- Claude Code's CLAUDE.md can reference KB lookups: "Search the KB before modifying shared files"
