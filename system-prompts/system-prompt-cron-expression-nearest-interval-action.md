# System Prompt: cron-expression-nearest-interval-action

- Source: inline

## Summary

Multiple prompts (3)

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

${EXPR_6}

${EXPR_7}

${EXPR_8}

${EXPR_9}

## Action

${NUM}. Convert `${EXPR_10}` to a ${NUM}-field cron expression. Supported suffixes: `s` → ceil to nearest minute, `m` (minutes), `h` (hours), `d` (days). Examples: `5m` → `*/${NUM} * * * *`, `1h` → `${NUM} * * * *`, `1d` → `${NUM} ${NUM} * * *`. If the interval doesn't cleanly divide its unit, round to the nearest clean interval and tell the user what you rounded to.
${NUM}. Call ${EXPR_11} with:
   - `cron`: the expression from step ${NUM}
   - `prompt`: the literal string `${EXPR_12}` — ${EXPR_13}
   - `recurring`: `true`
${NUM}. Briefly confirm: ${EXPR_14}
${NUM}. **Then immediately run ${EXPR_15} now**, following the instructions inlined below. Don't wait for the first cron fire.

${EXPR_16}

${EXPR_17}
