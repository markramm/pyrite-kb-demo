---
id: plugins-and-extensions
type: note
title: "Plugins and Extensions"
tags: [plugins, extensions, customization]
importance: 7
---

Pyrite's plugin system lets you add domain-specific entry types, MCP tools, CLI commands, validators, and workflows.

## Built-in plugins

| Plugin | Use case | Entry types added |
|--------|----------|-------------------|
| **software-kb** | Software project management | ADR, component, backlog_item, standard, runbook |
| **journalism-investigation** | Investigative journalism | claim, evidence, source (with reliability tiers) |
| **zettelkasten** | Personal knowledge management | Notes with maturity workflow |
| **cascade** | Timeline research | timeline_event, actor, capture lanes |
| **encyclopedia** | Reference articles | Articles with review workflow |
| **social** | Social engagement | Engagement tracking |

## Installing plugins

```bash
pip install pyrite-software-kb
pip install pyrite-journalism-investigation
```

Plugins register via Python entry points and are discovered automatically.

## Init templates

Plugins provide templates for `pyrite init`:

```bash
pyrite init --template software --path my-project
pyrite init --template zettelkasten --path my-notes
pyrite init --template research --path my-investigation
```

## Building your own

Plugins are Python packages that implement the `PyritePlugin` protocol. See the [plugin writing tutorial](https://pyrite.wiki/docs/plugin-protocol) for a step-by-step guide.

A plugin can provide:
- Custom entry types with validated fields
- MCP tools (read, write, and admin tier)
- CLI commands
- Validators and quality checks
- Relationship types
- Init templates (presets)
- Lifecycle hooks (before/after save)
