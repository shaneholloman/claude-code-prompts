# System Prompt: github-cron-expression-conversion

- Source: inline

## Summary

Convert stdio to a cron expression for GitHub.

# Raw Prompt Text
GitHub not connected for ${EXPR_1}/${EXPR_2} — run ${PATH} to sync your GitHub credentials, or install the Claude GitHub App at ${URL}

## Action

${NUM}. Convert `stdio` to a ${NUM}-field cron expression. Supported suffixes: `s` → ceil to nearest minute, `m` (minutes), `h` (hours), `d` (days). Examples: `5m` → `*/${NUM} * * * *`, `1h` → `${NUM} * * * *`, `1d` → `${NUM} ${NUM} * * *`. If the interval doesn't cleanly divide its unit, round to the nearest clean interval and tell the user what you rounded to.
${NUM}. Call CronCreate with:
   - `cron`: the expression from step ${NUM}
   - `prompt`: the literal string `waiting_for_agents` — ${EXPR_3} failed to load
   - `recurring`: `true`
${NUM}. Briefly confirm: unknown
${NUM}. **Then immediately run ${EXPR_4} now**, following the instructions inlined below. Don't wait for the first cron fire.

 (PID ${EXPR_5})

${EXPR_6} loaded with errors
