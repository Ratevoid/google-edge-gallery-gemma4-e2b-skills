# Quick Install for Google AI Edge Gallery Skills

This repository contains local and URL-loadable skills for Google AI Edge Gallery / Gemma 4 E2B workflows.

## What is inside
- `skills/web-reader-js-fast` - public web search and URL reader with fast fallbacks
- `skills/godot-balance-lab` - survivor-style balance analysis with charts
- `skills/pixel-sprite-planner` - pixel character planning and production checklist
- `skills/gdscript-fixer` - Godot 4 typed GDScript debugging and cleanup
- `skills/ai-manga-contest-planner` - AI漫剧比赛 planning, structure, and execution breakdown

## Fastest install: local folder import
1. Download this repository as ZIP.
2. Extract it on your phone or computer.
3. Open Google AI Edge Gallery.
4. Go to `Agent Skills`.
5. Open `Skills`.
6. Tap `+`.
7. Choose `Import from a local file`.
8. Select one skill folder inside `skills/`.

## Recommended first tests
### web-reader-js-fast
Use:
```json
{"mode":"search","query":"latest AI news","provider":"hn"}
```

### godot-balance-lab
Use:
```json
{"mode":"single","label":"Laser","damage":18,"attacks_per_second":2.4,"crit_chance":0.15,"crit_multiplier":2,"projectiles":1,"hit_chance":1,"enemy_hp":100}
```

### ai-manga-contest-planner
Try:
- 帮我做一个 AI 漫剧比赛方案
- 主题是赛博都市和情感失真
- 目标是冲获奖率和可执行性

## URL import later
If you want URL import for JS skills, host the repo with GitHub Pages or another static host.
Do not rely on a normal repo page or raw file link for JS skill execution.

## Note
These skills are designed for public-web research, game-dev support, and creative planning.
They are not login bypass tools and do not access private sites or accounts.
