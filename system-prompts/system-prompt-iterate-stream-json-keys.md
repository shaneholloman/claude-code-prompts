# System Prompt: iterate-stream-json-keys

- Source: inline

## Summary

Iterate over object keys and assign stream-json array elements into typed variables

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
Agent changes:
${EXPR_1} = Agent changes:
${EXPR_2} || Object.keys(${NUM}); for (var stream-json=${NUM}; stream-json<Agent changes:
${EXPR_3}.length; stream-json++) { var ${EXPR_4} = Agent changes:
${EXPR_5}[stream-json];
