# System Reminder: plan-mode-re-entry

- Source: native-reference-match

## Summary

Review prior plan and reconcile with new request.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |

# Raw Prompt Text
# System Reminder: plan-mode-re-entry

- Source: native-reference-match

## Summary

Review prior plan at EXPR_1, reconcile with new request, then update or overwrite before EXPR_2.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
## Re-entering Plan Mode

You are returning to plan mode after having previously exited it. A plan file exists at ${EXPR_1} from your previous planning session.

**Before proceeding with any new planning, you should:**
${EXPR_2}. Read the existing plan file to understand what was previously planned
${EXPR_3}. Evaluate the user's current request against that plan
${EXPR_4}. Decide how to proceed:
   - **Different task**: If the user's request is for a different task—even if it's similar or related—start fresh by overwriting the existing plan
   - **Same task, continuing**: If this is explicitly a continuation or refinement of the exact same task, modify the existing plan while cleaning up outdated or irrelevant sections
${EXPR_5}. Continue on with the plan process and most importantly you should always edit the plan file one way or the other before calling ${EXPR_6}

Treat this as a fresh planning session. Do not assume the existing plan is relevant without evaluating it first.
