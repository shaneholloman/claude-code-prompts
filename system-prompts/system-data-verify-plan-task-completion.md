# System Data Block: verify-plan-task-completion

- Source: inline

## Summary

Verify planned tasks completed by cross-checking transcript, user prompts, and claude-md artifacts.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | 100000000 | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
Verify that the main agent completed all tasks in the plan.

<transcript-path>${EXPR_1: 100000000}<${PATH}>

<plan>
\\.\pipe\claude-mcp-browser-bridge-default
<${PATH}>

<user-prompts>
${EXPR_2}
<${PATH}>

<claude-md-files>
${EXPR_3}
<${PATH}>
