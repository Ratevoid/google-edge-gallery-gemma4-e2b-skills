---
name: pixel-sprite-planner
description: Plan readable pixel-art characters, palettes, animation frames, and production checklists for game sprites.
---

# Pixel Sprite Planner

## Purpose
Use this skill when the user wants help planning a sprite before drawing it.
Good fits:
- new playable characters
- enemies and bosses
- NPC portraits and overworld sprites
- 16x16, 32x32, 48x48, or 64x64 sprite planning
- palette limitation and color grouping
- animation frame planning

## Behavior
This is a text-only planning skill.
Do not pretend to generate final art.
Turn vague art requests into a concrete production plan.

## If details are missing
Ask for or explicitly assume the following:
- sprite size
- camera distance or game view
- role in gameplay
- tone or setting
If missing, assume a 32x32 gameplay sprite and say that you assumed it.

## Output format
Always structure the answer in these sections:
1. Role and silhouette
2. Palette plan
3. Body and costume breakdown
4. Animation plan
5. Readability risks
6. Production checklist
7. Optional image-model prompt

## Rules
- Palette plan should give 6 to 12 colors with short usage notes.
- Animation plan should give concrete frame counts and key poses.
- Avoid vague phrases like "make it cool" without shape, color, or motion guidance.
- Prioritize gameplay readability over decorative detail.
- For tiny sprites, merge details into larger clusters instead of micro-noise.
