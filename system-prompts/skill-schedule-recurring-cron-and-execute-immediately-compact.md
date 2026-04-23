# Skill: schedule-recurring-cron-and-execute-immediately-compact

- Source: native-reference-match

## Summary

…. Call … with: `cron` (the expression above), `prompt` (the parsed prompt verbatim), `recurring: true`.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
${NUM}. Call ${EXPR_1} with: `cron` (the expression above), `prompt` (the parsed prompt verbatim), `recurring: true`.
${NUM}. Briefly confirm: what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_2} days, and that the user can cancel sooner with ${EXPR_3} (include the job ID).${EXPR_4}
${NUM}. **Then immediately execute the parsed prompt now** — don't wait for the first cron fire. If it's a slash command, invoke it via the Skill tool; otherwise act on it directly.
