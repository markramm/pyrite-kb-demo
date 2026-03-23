---
id: understanding-entry-types
type: note
title: "Understanding Entry Types"
tags: [concepts, schema, types]
importance: 8
---

Every entry in Pyrite has a type. Types define what fields an entry has, where its file lives, and how it's validated.

## Built-in types

Pyrite ships with 10 core types:

| Type | Purpose | Key fields |
|------|---------|------------|
| **note** | General-purpose notes | tags |
| **person** | People | role, affiliations |
| **organization** | Companies, institutions | org_type |
| **event** | Things that happened | date, location, participants |
| **document** | Documents and artifacts | doc_type, author |
| **topic** | Concepts and themes | — |
| **relationship** | Connections between entities | source, target, relation |
| **timeline** | Chronological events | date |
| **collection** | Groups of entries | source_type, query |
| **qa_assessment** | Quality assessments | target, rules, score |

## Plugin types

Plugins add domain-specific types. For example:

- **software-kb**: `adr`, `component`, `backlog_item`, `standard`, `runbook`
- **journalism-investigation**: `claim`, `evidence`, `source` (with reliability tiers)
- **zettelkasten**: Notes with maturity workflow (capture → elaborate → question → refine → connect)
- **cascade**: `timeline_event`, `actor`, capture lanes

## Custom types via kb.yaml

Define your own types in `kb.yaml`:

```yaml
types:
  recipe:
    description: "A cooking recipe"
    subdirectory: recipes
    fields:
      cuisine:
        type: string
        required: true
      prep_time:
        type: string
      servings:
        type: integer
```

Pyrite validates entries against their type schema on every write.

## How types affect the UI

- The **entries page** shows a type filter dropdown
- The **graph view** colors nodes by type
- The **orient page** shows type breakdown with counts
- **Search** can filter by type: `pyrite search "query" --type person`
