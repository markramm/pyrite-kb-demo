---
id: getting-started
type: note
title: "Getting Started"
tags: [getting-started, install, cli]
importance: 9
---

Get from zero to a working knowledge base in five minutes.

## Install

```bash
pip install pyrite                # Core
pip install "pyrite[all]"         # Core + AI + semantic search
```

## Create a knowledge base

```bash
pyrite init --template research --path my-kb
cd my-kb
```

Templates available: `research`, `software`, `zettelkasten`, `intellectual-biography`, `movement`, `empty`.

## Add entries

```bash
pyrite create -k my-kb --type person --title "Ada Lovelace" \
  --body "Mathematician and writer. First algorithm." --tags "computing"

pyrite create -k my-kb --type note --title "Research notes" \
  --body "Key finding: [[ada-lovelace]] anticipated modern computing."
```

Wikilinks like `[[ada-lovelace]]` automatically create connections in the knowledge graph.

## Search

```bash
pyrite search "algorithm" -k my-kb                    # keyword
pyrite search "early computing" -k my-kb --mode semantic   # meaning-based
pyrite search "computing" -k my-kb --mode hybrid      # both
```

## Start the web UI

```bash
pyrite-server
# Visit http://localhost:8088
```

## Connect your AI

See [[connecting-via-mcp]] for Claude, OpenAI, and Gemini configuration.

## What was created

```
my-kb/
  kb.yaml           # KB configuration and type definitions
  person/
    ada-lovelace.md  # Entry files with YAML frontmatter
  note/
    research-notes.md
  .pyrite/
    index.db         # Search index (derived, rebuildable)
```

Your files are the source of truth. The index is derived. Rebuild it anytime with `pyrite index build`.
