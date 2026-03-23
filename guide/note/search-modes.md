---
id: search-modes
type: note
title: "Search Modes"
tags: [search, concepts, semantic]
importance: 8
---

Pyrite supports three search modes, each suited to different needs.

## Keyword search (default)

Finds entries containing your exact terms. Uses SQLite FTS5 with BM25 ranking.

```bash
pyrite search "knowledge management" -k my-kb
```

Best for: finding specific entries, known terms, exact phrases.

## Semantic search

Finds conceptually related content using vector embeddings. Requires `pyrite[semantic]` installed.

```bash
pyrite search "how to organize research" -k my-kb --mode semantic
```

Best for: exploratory queries, finding related concepts, natural language questions.

## Hybrid search

Combines keyword and semantic results using Reciprocal Rank Fusion (RRF). Gets the best of both approaches.

```bash
pyrite search "policy implications" -k my-kb --mode hybrid
```

Best for: most queries — it finds exact matches AND conceptually related entries.

## Filtering

Narrow results by type, tag, or KB:

```bash
pyrite search "encryption" --type person     # only people
pyrite search "encryption" --tag policy      # only tagged "policy"
pyrite search "encryption" -k schneier       # only in schneier KB
```

## In the web UI

The search page supports all three modes via a dropdown. Results show highlighted snippets with matched terms.

## In MCP

AI agents use `kb_search` with `mode` parameter:

```
kb_search(query="encryption policy", mode="hybrid", kb="schneier")
```
