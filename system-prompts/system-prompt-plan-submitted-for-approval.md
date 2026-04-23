# System Prompt: plan-submitted-for-approval

- Source: inline

## Summary

Informs that a plan was sent to a team lead and must be approved before proceeding.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | @anthropic-ai/claude-code | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
Your plan has been submitted to the team lead for approval.

Plan file: ${EXPR_1}

**What happens next:**
${NUM}. Wait for the team lead to review your plan
${NUM}. You will receive a message in your inbox with approval${PATH}
${NUM}. If approved, you can proceed with implementation
${NUM}. If rejected, refine your plan based on the feedback

**Important:** Do NOT proceed until you receive approval. Check your inbox for response.

Request ID: npm view ${EXPR_2: '@anthropic-ai/claude-code'}@${EXPR_3} version
