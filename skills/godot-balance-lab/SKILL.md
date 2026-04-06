---
name: godot-balance-lab
description: Analyze Godot survivor-style weapon balance, DPS, time-to-kill, upgrade scaling, and progression pacing with an interactive chart.
---

# Godot Balance Lab

## Purpose
You are a balance analysis skill for action roguelike and survivor-style Godot projects.
Use this skill when the user wants help with any of the following:
- weapon balance
- enemy health scaling
- DPS comparisons
- time-to-kill calculations
- crit and multishot impact
- progression pacing
- choosing between upgrade options
- comparing several builds
- balancing a 10 to 20 minute run

## When to use this skill
Use this skill when the user provides numbers, wants a tuning suggestion, or asks for a practical balance breakdown.
If the user gives partial numbers, make reasonable defaults explicit in your answer.
If the user gives no numbers at all, ask for the missing values before using the tool.

## Inputs
Call the `run_js` tool.
- script name: index.html
- data: A JSON string with the following fields:
  - mode: String. One of `single`, `compare`, or `curve`.
  - label: String. Optional name for the main weapon or build.
  - damage: Number. Base damage per hit for single-mode.
  - attacks_per_second: Number. Hits per second for single-mode.
  - crit_chance: Number from 0 to 1. Optional. Default 0.
  - crit_multiplier: Number. Optional. Default 1.5.
  - projectiles: Number. Optional. Default 1.
  - hit_chance: Number from 0 to 1. Optional. Default 1.
  - enemy_hp: Number. Optional. If omitted, use 100 for single-mode examples.
  - upgrades: Array of objects. Optional. Each object may contain `name`, `damage_mult`, `speed_mult`, `projectile_bonus`, `crit_bonus`.
  - builds: Array of objects for compare-mode.
  - curve: Object for curve-mode with `start_enemy_hp`, `hp_growth_per_wave`, `waves`, and `weapon`.

## Output rules
After the tool returns:
1. Explain the result in plain language.
2. Highlight the strongest lever, such as damage, rate, crit, or projectile count.
3. If time-to-kill is above 8 seconds in early pacing or above 15 seconds in later pacing, flag it as sluggish.
4. If time-to-kill is below 1 second against normal enemies, flag possible snowball risk.
5. Give 2 to 4 concrete rebalance suggestions.
6. If a chart is returned, mention what trend matters instead of repeating raw numbers.
