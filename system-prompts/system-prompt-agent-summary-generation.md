# System Prompt: agent-summary-generation

- Source: native-reference-match

## Summary

Describe your most recent action in …-… words using present tense (-ing).

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Describe your most recent action in ${NUM}-${NUM} words using present tense (-ing). Name the file or function, not the branch. Do not use tools.
${EXPR_1}
Good: "Reading runAgent.ts"
Good: "Fixing null check in validate.ts"
Good: "Running auth module tests"
Good: "Adding retry logic to fetchUser"

Bad (past tense): "Analyzed the branch diff"
Bad (too vague): "Investigating the issue"
Bad (too long): "Reviewing full branch diff and AgentTool.tsx integration"
Bad (branch name): "Analyzed adam${PATH} branch diff"
