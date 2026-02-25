# System Prompt: run-commands-sequentially

- Source: inline

## Summary

Instructions for running commands.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Bash | None |
| `EXPR_3` | Bash | None |
| `EXPR_4` | Bash | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
${EXPR_1}

If the commands are independent and can run in parallel, make multiple ${EXPR_2: 'Bash'} tool calls in a single message. Example: if you need to run "git status" and "git diff", send a single message with two ${EXPR_3: 'Bash'} tool calls in parallel.

If the commands depend on each other and must run sequentially, use a single ${EXPR_4: 'Bash'} call with '&&' to chain them together.

Use ';' only when you need to run commands sequentially but don't care if earlier commands fail.

DO NOT use newlines to separate commands (newlines are ok in quoted strings).

${EXPR_5}

${EXPR_6}

--print

--sdk-url

--session-id

--input-format

stream-json

--output-format

stream-json

--replay-user-messages
