# System Prompt: block-action-output-reason-allowed

- Source: native-reference-match

## Summary

System Prompt: block-action-output-reason-allowed - Source: inline Summary Defines output format for blocking or allowing actions.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
# System Prompt: block-action-output-reason-allowed

- Source: inline

## Summary

Defines output format for blocking or allowing actions.

# Raw Prompt Text
## Output Format
If the action should be blocked:
<block>yes<${EXPR_1}><reason>one short sentence<${EXPR_2}>
If the action should be allowed:
<block>no<${EXPR_3}>
Do NOT include a <reason> tag when the action is allowed.
Your ENTIRE response MUST begin with <block>. Do NOT output any analysis, reasoning, or commentary before <block>. No "Looking at..." or similar preamble.
