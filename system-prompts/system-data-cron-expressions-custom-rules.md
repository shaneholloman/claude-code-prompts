# System Data Block: cron-expressions-custom-rules

- Source: inline

## Summary

Convert custom rules to cron expressions.

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
| `EXPR_10` | None | None |
| `EXPR_11` | CronDelete | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |

# Raw Prompt Text
pr-${EXPR_1}

## Action

${NUM}. Convert `## allow (custom rules replacing defaults)
Custom:
${EXPR_2}

Defaults being replaced:
${EXPR_3}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_4}

Defaults being replaced:
${EXPR_5}

## environment (custom rules replacing defaults)
Custom:
${EXPR_6}

Defaults being replaced:
${EXPR_7}

` to a ${NUM}-field cron expression. Supported suffixes: `s` → ceil to nearest minute, `m` (minutes), `h` (hours), `d` (days). Examples: `5m` → `*/${NUM} * * * *`, `1h` → `${NUM} * * * *`, `1d` → `${NUM} ${NUM} * * *`. If the interval doesn't cleanly divide its unit, round to the nearest clean interval and tell the user what you rounded to.
${NUM}. Call CronCreate with:
   - `cron`: the expression from step ${NUM}
   - `prompt`: the literal string `${EXPR_8} loaded with errors` — ${EXPR_9}
   - `recurring`: `true`
${NUM}. Briefly confirm: what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_10} days, and that they can cancel sooner with ${EXPR_11: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
${NUM}. **Then immediately run ${EXPR_12} now**, following the instructions inlined below. Don't wait for the first cron fire.

brew upgrade ${EXPR_13}

 (PID ${EXPR_14})
