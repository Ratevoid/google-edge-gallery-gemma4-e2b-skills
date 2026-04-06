---
name: web-reader-js-fast
description: Fast JavaScript web search and public URL reader for AI Edge Gallery. Always use run_js. Never use run_intent. Prefer provider wikipedia or hn for speed; use jina only when needed.
homepage: "https://github.com/google-ai-edge/gallery/tree/main/skills"
---

# Web Reader JS Fast

This is a JavaScript skill for AI Edge Gallery.

## Critical rule
- Always call `run_js`
- Never call `run_intent`
- Never use native intents such as `search_web`

## Use cases
- search the public web quickly
- read a public webpage or PDF from a URL
- get fast fallback results when generic web search is slow

## Fast tip
For best reliability on mobile:
- use `provider: "wikipedia"` for broad facts
- use `provider: "hn"` for AI, news, and dev topics
- use `provider: "jina"` only when you need broader web search

## JSON formats
### Search
```json
{
  "mode": "search",
  "query": "your search query",
  "provider": "auto"
}
```

### Fast AI or news search
```json
{
  "mode": "search",
  "query": "latest AI news",
  "provider": "hn"
}
```

### Fast general knowledge search
```json
{
  "mode": "search",
  "query": "Godot AnimationPlayer",
  "provider": "wikipedia"
}
```

### Read a public URL
```json
{
  "mode": "read",
  "url": "https://example.com/page"
}
```
