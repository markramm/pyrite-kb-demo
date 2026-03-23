---
id: web-ui-features
type: note
title: "Web UI Features"
tags: [web, getting-started, concepts]
importance: 7
---

Pyrite's web UI is a SvelteKit application that provides a visual interface to your knowledge bases. Start it locally with `pyrite-server` or access it on a hosted deployment like this demo.

## Pages

### Dashboard
The home page shows global stats (KB count, total entries, tags, links), recent entries, entry type distribution chart, and a list of all KBs. Click a KB name to see its orientation page.

### Entries
Browse and filter entries by KB, type, and tags. Click an entry to view its full content with rendered wikilinks, backlinks, metadata sidebar, and local graph. Entries are paginated (50 per page).

### Search
Full-text search across all KBs with mode selector (keyword, semantic, hybrid). Results show highlighted snippets with matched terms.

### Graph
Interactive knowledge graph visualization powered by Cytoscape.js. Nodes are colored by entry type, sized by link count. Click a node to navigate to the entry. Filter by KB and type, adjust depth, switch layouts (force-directed, circle, grid, concentric).

### Collections
Create and manage collections of entries — either folder-based or query-based. Collections support multiple view types.

### Timeline
Chronological view of entries with dates. Filter by date range and minimum importance.

### Orient
KB orientation page showing description, entry types with counts, top tags, guidelines, and recent changes. This is what you see when you click a KB name from the dashboard.

### Settings
Configure AI API keys, manage KBs, view plugins, and adjust UI preferences.

## Editor

The entry editor supports dual-mode editing:

- **Rich text** (Tiptap) — WYSIWYG markdown editing with toolbar
- **Source** (CodeMirror) — direct markdown editing with syntax highlighting

Both modes support `[[wikilink]]` autocomplete — type `[[` and get suggestions from existing entries.

## Keyboard shortcuts

- `Cmd+K` — Quick switcher (navigate to any entry by name)
- `Cmd+Shift+K` — AI chat sidebar
- `Cmd+D` — Today's daily note
- `Cmd+/` — Toggle sidebar
- `?` — Keyboard shortcuts help
