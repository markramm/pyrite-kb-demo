---
id: local-install
type: note
title: "Installing Pyrite Locally"
tags: [getting-started, install, cli]
importance: 9
---

Pyrite runs on Python 3.11+ and installs via pip. No external services required.

## Basic install

```bash
pip install pyrite
```

This gives you the CLI, MCP server, and REST API. SQLite storage, no cloud dependencies.

## Full install (recommended)

```bash
pip install "pyrite[all]"
```

Includes everything: CLI, REST API server, AI provider SDKs (Anthropic, OpenAI), semantic search (sentence-transformers + sqlite-vec), and development tools.

## Install options

| Extra | What it adds | When you need it |
|-------|-------------|------------------|
| `pyrite[cli]` | Typer + Rich CLI | Always (included in core) |
| `pyrite[server]` | FastAPI, uvicorn, web UI | Running `pyrite-server` |
| `pyrite[ai]` | Anthropic + OpenAI + Gemini SDKs | AI features (summarize, auto-tag, chat) |
| `pyrite[semantic]` | sentence-transformers, sqlite-vec | Semantic and hybrid search |
| `pyrite[all]` | Everything above + dev tools | Recommended for most users |

## Verify installation

```bash
pyrite --help          # CLI works
pyrite-server --help   # Server works
pyrite mcp --help      # MCP server works
```

## Create your first KB

```bash
pyrite init --template research --path my-kb
cd my-kb
```

See [[getting-started]] for a full walkthrough.

## System requirements

- Python 3.11, 3.12, or 3.13
- ~500MB disk for semantic search models (downloaded on first use)
- No GPU required — CPU inference works fine for the embedding model
