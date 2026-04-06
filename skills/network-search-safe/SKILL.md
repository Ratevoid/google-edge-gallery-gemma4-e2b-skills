---
name: network-search-safe
description: Reliable public-web search for AI Edge Gallery. Always use run_js. Never use run_intent. Prefer Wikipedia and Hacker News first because they are lighter and more stable on mobile.
---

# Network Search Safe

## Purpose
This skill is designed to make public-web lookup more reliable inside AI Edge Gallery.
It is intentionally conservative.
It avoids native intents and tries lightweight sources first.

## Critical rules
- Always call `run_js`
- Never call `run_intent`
- Never use native intents such as `search_web`
- Prefer `wikipedia` or `hn` when the user is asking for broad facts, docs, AI topics, or recent tech discussion
- Use `jina` only when the user explicitly wants broader web search or URL reading

## Best-use cases
- public web facts
- docs lookup
- AI and developer news
- reading public pages and public PDFs

## Supported modes
### 1. Search
```json
{
  "mode": "search",
  "query": "Godot AnimationPlayer",
  "provider": "auto"
}
```

### 2. Wikipedia-first search
```json
{
  "mode": "search",
  "query": "Godot",
  "provider": "wikipedia"
}
```

### 3. Hacker News-first search
```json
{
  "mode": "search",
  "query": "latest AI news",
  "provider": "hn"
}
```

### 4. Read a public URL
```json
{
  "mode": "read",
  "url": "https://docs.godotengine.org/en/stable/"
}
```

## Notes
- This skill is for public web content only.
- It does not access private accounts, logins, or paywalled content.
- For first-time testing, send JSON directly instead of a loose natural-language sentence.
