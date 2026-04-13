# System Prompt: cron-expression-github-sync

- Source: inline

## Summary

Convert local time to cron expression for GitHub.

# Raw Prompt Text
GitHub not connected for ${EXPR_1}/${EXPR_2} — run ${PATH} to sync your GitHub credentials, or install the Claude GitHub App at ${URL}

## Action

${NUM}. Convert `local` to a ${NUM}-field cron expression. Supported suffixes: `s` → ceil to nearest minute, `m` (minutes), `h` (hours), `d` (days). Examples: `5m` → `*/${NUM} * * * *`, `1h` → `${NUM} * * * *`, `1d` → `${NUM} ${NUM} * * *`. If the interval doesn't cleanly divide its unit, round to the nearest clean interval and tell the user what you rounded to.
${NUM}. Call CronCreate with:
   - `cron`: the expression from step ${NUM}
   - `prompt`: the literal string `${EXPR_3} loaded with errors` — ${EXPR_4}
   - `recurring`: `true`
${NUM}. Briefly confirm: what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_5} days, and that they can cancel sooner with ${EXPR_6} (include the job ID). Mention this is the autonomous default and that the autonomous-loop instructions are baked in.
${NUM}. **Then immediately run ${EXPR_7} now**, following the instructions inlined below. Don't wait for the first cron fire.

 (PID ${EXPR_8})

${EXPR_9}
