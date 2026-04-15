# System Data Block: custom-rules-github-cron

- Source: inline

## Summary

Customize cron rules for GitHub integration.

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
| `EXPR_11` | None | None |
| `EXPR_12` | CronDelete | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |

# Raw Prompt Text
GitHub not connected for ${EXPR_1}/${EXPR_2} — run ${PATH} to sync your GitHub credentials, or install the Claude GitHub App at ${URL}

## Action

${NUM}. Convert `## allow (custom rules replacing defaults)
Custom:
${EXPR_3}

Defaults being replaced:
${EXPR_4}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_5}

Defaults being replaced:
${EXPR_6}

## environment (custom rules replacing defaults)
Custom:
${EXPR_7}

Defaults being replaced:
${EXPR_8}

` to a ${NUM}-field cron expression. Supported suffixes: `s` → ceil to nearest minute, `m` (minutes), `h` (hours), `d` (days). Examples: `5m` → `*/${NUM} * * * *`, `1h` → `${NUM} * * * *`, `1d` → `${NUM} ${NUM} * * *`. If the interval doesn't cleanly divide its unit, round to the nearest clean interval and tell the user what you rounded to.
${NUM}. Call CronCreate with:
   - `cron`: the expression from step ${NUM}
   - `prompt`: the literal string `${EXPR_9} loaded with errors` — ${EXPR_10}
   - `recurring`: `true`
${NUM}. Briefly confirm: what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_11} days, and that they can cancel sooner with ${EXPR_12: 'CronDelete'} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
${NUM}. **Then immediately run ${EXPR_13} now**, following the instructions inlined below. Don't wait for the first cron fire.

 (PID ${EXPR_14})

${EXPR_15}
