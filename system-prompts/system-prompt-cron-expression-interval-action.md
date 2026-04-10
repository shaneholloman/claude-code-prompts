# System Prompt: cron-expression-interval-action

## Summary

Convert intervals to cron expressions and execute actions.

# Raw Prompt Text
${EXPR_1}

## Action

${NUM}. Convert `stdio` to a ${NUM}-field cron expression. Supported suffixes: `s` → ceil to nearest minute, `m` (minutes), `h` (hours), `d` (days). Examples: `5m` → `*/${NUM} * * * *`, `1h` → `${NUM} * * * *`, `1d` → `${NUM} ${NUM} * * *`. If the interval doesn't cleanly divide its unit, round to the nearest clean interval and tell the user what you rounded to.
${NUM}. Call CronCreate with:
   - `cron`: the expression from step ${NUM}
   - `prompt`: the literal string `waiting_for_agents` — ${EXPR_2} failed to load
   - `recurring`: `true`
${NUM}. Briefly confirm: unknown
${NUM}. **Then immediately run ${EXPR_3} now**, following the instructions inlined below. Don't wait for the first cron fire.

 (PID ${EXPR_4})

${EXPR_5} loaded with errors
