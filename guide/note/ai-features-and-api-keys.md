---
id: ai-features-and-api-keys
type: note
title: "AI Features and API Key Configuration"
tags: [ai, configuration, getting-started]
importance: 8
---

Pyrite includes optional AI-powered features that require an API key from Anthropic, OpenAI, or Google. All AI features are BYOK (Bring Your Own Key) — nothing runs without your explicit configuration.

## What AI features are available

| Feature | What it does | Where it appears |
|---------|-------------|-----------------|
| **Summarize** | Generate a summary of an entry | Entry page toolbar |
| **Auto-tag** | Suggest tags based on content | Entry page toolbar |
| **Chat sidebar** | Ask questions about the KB | Cmd+Shift+K |
| **Semantic search** | Find by meaning, not just keywords | Search page, CLI |

Semantic search uses a **local model** (sentence-transformers) and does NOT require an API key. The other features use cloud LLM APIs.

## Configuring API keys

### In the web UI

Go to **Settings** (gear icon in sidebar) and enter your API key:

- **Anthropic API key**: For Claude-powered summarize, auto-tag, and chat
- **OpenAI API key**: Alternative provider for the same features
- **Google API key**: For Gemini-powered features

Settings are stored locally in the browser and sent with each request. They are NOT stored on the server.

### Via environment variables

For CLI and server deployments:

```bash
export ANTHROPIC_API_KEY=sk-ant-...
export OPENAI_API_KEY=sk-...
export GEMINI_API_KEY=...
```

Or in a `.env` file in your project directory.

### Via config

In `~/.pyrite/config.yaml` or your KB's settings:

```yaml
settings:
  ai:
    provider: anthropic          # or openai, gemini
    model: claude-sonnet-4-20250514
```

## No AI? No problem

Pyrite works fully without any AI features:

- **Keyword search** works out of the box (FTS5, no model needed)
- **Semantic search** uses a local model — no API key, no cloud calls
- **All CRUD operations** work via CLI, REST API, and MCP
- **The web UI** works completely without AI keys — you just won't see the summarize/tag/chat buttons

## Privacy

- API keys entered in the UI are stored in your browser's localStorage only
- The Pyrite server proxies AI requests — your content is sent to the AI provider you configured
- If you don't configure an AI provider, zero content leaves your machine
- Self-hosted deployments never send data anywhere unless you explicitly configure an AI provider
