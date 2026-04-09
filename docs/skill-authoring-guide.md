# Skill Authoring Guide

This repo is meant for small, testable skills that work well with local Gemma-style usage in Google AI Edge Gallery.

## Goal

A good skill should help someone get from vague input to useful output fast.

## The basic shape

Every skill should contain:

1. Purpose
2. Use when
3. Input
4. Output format
5. Prompt
6. Success check

## Design rules

### 1. One skill, one job
Do not make a skill that writes, plans, critiques, translates, and formats all at once.

### 2. Short inputs win
Skills should work with light context. Assume the user is on-device and wants speed.

### 3. Structured output beats pretty output
Use sections, lists, or tables. The user should know where to look.

### 4. Success must be testable
A skill should have a visible sign of success, not just “it sounds smart.”

## Bad pattern
- huge prompt
- vague mission
- no output structure
- no example

## Better pattern
- narrow problem
- fixed output
- obvious use case
- one example nearby

## Recommended test
Run the same skill on 3 different inputs.
If the result stays useful and structured, the skill is strong enough to keep.
