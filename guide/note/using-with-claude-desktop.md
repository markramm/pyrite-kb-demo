---
id: using-with-claude-desktop
type: note
title: "Using Pyrite with Claude Desktop and Cowork"
tags: [claude, mcp, getting-started]
importance: 9
---

Claude Desktop (chat) and Claude Cowork (collaborative agent) both support MCP servers. Connecting Pyrite gives Claude persistent memory across conversations.

## Claude Desktop setup

1. Install Pyrite locally: `pip install "pyrite[all]"` (see [[local-install]])
2. Edit your Claude Desktop config:

**macOS**: `~/Library/Application Support/Claude/claude_desktop_config.json`
**Windows**: `%APPDATA%\Claude\claude_desktop_config.json`

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

3. Restart Claude Desktop

## What this enables

Claude can now:

- **Search your knowledge**: "What do I know about Bruce Schneier's work on trust?"
- **Read specific entries**: "Show me the entry on security theater"
- **Create new knowledge**: "Save this as a note about our meeting discussion"
- **Follow connections**: "What links to the entry about surveillance economics?"
- **Cross-KB queries**: Search across all your registered knowledge bases

## Claude Cowork

Cowork uses the same MCP configuration. When working in Cowork mode, multiple Claude instances can read and write the same KB, enabling collaborative knowledge building.

## Example conversations

**Research assistant:**
> "I'm researching encryption policy. Search my research KB for anything related."
> Claude searches, finds entries, synthesizes across them.

**Personal knowledge management:**
> "I just read an article about systems thinking. Create a note capturing the key ideas and link it to my existing entry on feedback loops."
> Claude creates the entry with wikilinks to related concepts.

**Team knowledge:**
> "What decisions have we made about the API design? Check the ADRs."
> Claude searches for ADR entries and summarizes the decisions.

## Read-only mode

If you only want Claude to read (not create or modify entries):

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

## Multiple KBs

Pyrite's MCP server exposes all registered KBs. Claude can search across all of them or target a specific one:

> "Search the schneier KB for entries about cryptography"
> "Create a note in my research KB about today's findings"
