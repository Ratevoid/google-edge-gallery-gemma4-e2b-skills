# Output Format Enforcer Example

## Input
- Task: turn a rough idea into a short video concept
- Required sections: Hook, Conflict, Ending, Visual Beat
- Forbidden output: long paragraphs, changing headings
- Example of ideal structure: 4 fixed sections with short text

## Example result
### Format diagnosis
The request is clear, but the output shape is too loose.

### Revised instruction block
Return exactly 4 sections with these headings: Hook, Conflict, Ending, Visual Beat.

### Minimal output schema
- Hook:
- Conflict:
- Ending:
- Visual Beat:

## Why it works
- the model has fewer ways to drift
- repeated tests become easier to compare
- the output is easier to reuse in a workflow
