---
id: knowledge-graph
type: note
title: "Knowledge Graph"
tags: [graph, wikilinks, concepts]
importance: 7
---

Pyrite automatically builds a knowledge graph from the links between your entries. The graph view visualizes connections, helping you discover relationships and structural patterns.

## How links work

Links are created by using `[[wikilink]]` syntax in entry bodies:

```markdown
[[ada-lovelace]] anticipated the capabilities of [[charles-babbage]]'s
Analytical Engine, writing what is considered the first [[algorithm]].
```

Each `[[target-id]]` becomes a directed edge in the graph. Pyrite tracks both outgoing links and backlinks automatically.

## The graph view

The web UI graph page (`/graph`) renders an interactive force-directed graph using Cytoscape.js:

- **Nodes** are colored by entry type (person=purple, concept=gray, event=blue, etc.)
- **Node size** scales with link count — highly connected entries are larger
- **Click a node** to navigate to that entry
- **Hover** to see title, type, and link count
- **Search** to highlight matching nodes
- **Filter** by KB or entry type

## Graph controls

- **KB**: Show entries from one KB or all
- **Type**: Filter to specific entry types
- **Depth**: How many hops from linked entries to include (1-3)
- **Layout**: Force-directed (default), circle, grid, or concentric

## Backlinks

Every entry page shows its backlinks — all entries that link TO this entry. This is one of the most valuable features for discovery: you can see what references any given concept, person, or event.

## CLI

```bash
pyrite backlinks ada-lovelace -k my-kb    # what links to this entry?
pyrite get ada-lovelace -k my-kb          # entry with outlinks listed
```
