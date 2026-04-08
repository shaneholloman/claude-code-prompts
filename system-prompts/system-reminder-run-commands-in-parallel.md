# System Prompt: run-commands-in-parallel

- Source: inline

## Summary

Multiple prompts (2)

# Raw Prompt Text
If the commands are independent and can run in parallel, make multiple ${EXPR_1} tool calls in a single message. Example: if you need to run "git status" and "git diff", send a single message with two ${EXPR_2} tool calls in parallel.

If the commands depend on each other and must run sequentially, use a single ${EXPR_3} call with '&&' to chain them together.

Use ';' only when you need to run commands sequentially but don't care if earlier commands fail.

DO NOT use newlines to separate commands (newlines are ok in quoted strings).

stream-json
