# Skill: schedule-recurring-cron-and-run-immediately

- Source: native-reference-match

## Summary

Convert intervals to cron expressions and execute actions.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |

# Raw Prompt Text
${EXPR_1}

## Action

${NUM}. Convert `${EXPR_2}` to a ${NUM}-field cron expression. Supported suffixes: `s` → ceil to nearest minute, `m` (minutes), `h` (hours), `d` (days). Examples: `5m` → `*/${NUM} * * * *`, `1h` → `${NUM} * * * *`, `1d` → `${NUM} ${NUM} * * *`. If the interval doesn't cleanly divide its unit, round to the nearest clean interval and tell the user what you rounded to.
${NUM}. Call ${EXPR_3} with:
   - `cron`: the expression from step ${NUM}
   - `prompt`: the literal string `${EXPR_4}` — ${EXPR_5}
   - `recurring`: `true`
${NUM}. Briefly confirm: ${EXPR_6}
${NUM}. **Then immediately run ${EXPR_7} now**, following the instructions inlined below. Don't wait for the first cron fire.

${EXPR_8}

${EXPR_9}
