# Workflow

## Decision Rules

How to choose between options:

1. **Match Domain First:** Select suggestions that align most closely with the specified domain
2. **Tie-Breaker by Simplicity:** If multiple suggestions fit equally, output all with reasoning
3. **Fallback:** If no match found, reply with "No suggestion found" and explain why

## Missing Input Handling

- No question/scenario provided → Prompt user to clarify
- No domain provided → Ask user to specify domain

## Stopping Conditions

When the skill's task is complete:

| Condition | Threshold | Action |
|-----------|-----------|--------|
| Lack of Required Input | 3 prompts | End interaction |
| Refinement Limit | 3 refinements | Output final suggestion, end |
| User Confirmation | User satisfied | Task complete |

