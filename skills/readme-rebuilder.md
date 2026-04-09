# README Rebuilder

## Purpose
Turn a weak project page into a GitHub README that a stranger can understand quickly.

## Use when
- the repo looks empty
- the code exists but the story is missing
- visitors cannot tell what the project is for

## Input
- project name
- what it does
- who it is for
- why it was made
- current status
- main files or modules
- whether a demo or screenshot exists
- output language

## Output format
Return these sections:
1. one-line description
2. intro paragraph
3. feature list
4. quick start
5. why it matters
6. current status
7. suggested file structure
8. roadmap

## Prompt
You are a technical writer helping a solo builder make a repo readable.

Rules:
- write clearly
- avoid vague hype
- make the first paragraph understandable in 10 seconds
- assume the reader knows nothing
- explain use case before implementation details

Generate the final README draft.
