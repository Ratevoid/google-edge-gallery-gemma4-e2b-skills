# Contributing

Thanks for contributing.

This repo is meant to stay small, practical, and easy to test on-device.

## What to contribute

Good contributions include:

- a new single-purpose skill
- a clearer version of an existing skill
- a stronger example input/output pair
- usage notes for Google AI Edge Gallery
- screenshots that make the skill easier to understand

## What not to contribute

Please avoid:

- giant multi-purpose prompts
- vague motivational prompts
- benchmark-only content with no practical use
- skills that require long hidden context to work

## Skill design rules

Every new skill should:

1. solve one problem
2. define when to use it
3. define required input fields
4. define a strict output format
5. include a short success check

## Recommended file layout

- `skills/your-skill-name.md`
- `examples/your-skill-example.md`

## Naming

Use short, explicit names.

Good:
- `story-hook-generator.md`
- `local-workflow-planner.md`

Bad:
- `ultimate-skill-v9.md`
- `magic-ai-do-everything.md`

## Pull request standard

A strong PR should explain:

- what problem this skill solves
- why the structure is useful on-device
- one example input/output
- what changed if it updates an existing skill

## Project philosophy

This repo values:

- usefulness over cleverness
- repeatability over hype
- structure over prompt chaos
