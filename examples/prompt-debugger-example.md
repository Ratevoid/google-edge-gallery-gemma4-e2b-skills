# Prompt Debugger Example

## Input
- Current prompt: Write a cool sci-fi short script.
- Example input: a delivery rider discovers his customers vanish the next day
- Bad output: generic, slow, no hook, no structure
- Expected output: a fast opening with conflict and cliffhanger

## Example result
### Main failure point
The prompt is too vague and gives the model no structural target.

### Why it happens
Words like "cool" and "short" are loose. The model fills space with generic sci-fi language.

### Revised prompt idea
Write a 30-second sci-fi thriller opening. Start with conflict in the first line, keep the language simple, and end on a cliffhanger.

## Why it works
- the failure becomes obvious
- the fix is small and reusable
- the result is easier to test again
