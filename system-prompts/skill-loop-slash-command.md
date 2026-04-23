# Skill: loop-slash-command

- Source: native-reference-match

## Summary

… — schedule a recurring prompt Parse the input below into `[interval] <prompt…>` and schedule it with ….

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

# Raw Prompt Text
# ${PATH} — schedule a recurring prompt

Parse the input below into `[interval] <prompt…>` and schedule it with ${EXPR_1}.

## Parsing (in priority order)

${NUM}. **Leading token**: if the first whitespace-delimited token matches `^\d+[smhd]$` (e.g. `5m`, `2h`), that's the interval; the rest is the prompt.
${NUM}. **Trailing "every" clause**: otherwise, if the input ends with `every <N><unit>` or `every <N> <unit-word>` (e.g. `every 20m`, `every ${NUM} minutes`, `every ${NUM} hours`), extract that as the interval and strip it from the prompt. Only match when what follows "every" is a time expression — `check every PR` has no interval.
${NUM}. **Default**: otherwise, interval is `${EXPR_2}` and the entire input is the prompt.

If the resulting prompt is empty, show usage `${PATH} [interval] <prompt>` and stop — do not call ${EXPR_3}.

Examples:
- `5m ${PATH}` → interval `5m`, prompt `${PATH}` (rule ${NUM})
- `check the deploy every 20m` → interval `20m`, prompt `check the deploy` (rule ${NUM})
- `run tests every ${NUM} minutes` → interval `5m`, prompt `run tests` (rule ${NUM})
- `check the deploy` → interval `${EXPR_4}`, prompt `check the deploy` (rule ${NUM})
- `check every PR` → interval `${EXPR_5}`, prompt `check every PR` (rule ${NUM} — "every" not followed by time)
- `5m` → empty prompt → show usage
${EXPR_6}
## Interval → cron

Supported suffixes: `s` (seconds, rounded up to nearest minute, min ${NUM}), `m` (minutes), `h` (hours), `d` (days). Convert:

| Interval pattern      | Cron expression     | Notes                                    |
|-----------------------|---------------------|------------------------------------------|
| `Nm` where N ≤ ${NUM}   | `*/N * * * *`     | every N minutes                          |
| `Nm` where N ≥ ${NUM}   | `${NUM} */H * * *`     | round to hours (H = N/${NUM}, must divide ${NUM})|
| `Nh` where N ≤ ${NUM}   | `${NUM} */N * * *`     | every N hours                            |
| `Nd`                | `${NUM} ${NUM} */N * *`     | every N days at midnight local           |
| `Ns`                | treat as `ceil(N/${NUM})m` | cron minimum granularity is ${NUM} minute  |

**If the interval doesn't cleanly divide its unit** (e.g. `7m` → `*/${NUM} * * * *` gives uneven gaps at :${NUM}→:${NUM}; `90m` → ${NUM}.5h which cron can't express), pick the nearest clean interval and tell the user what you rounded to before scheduling.

## Action

${NUM}. Call ${EXPR_7} with:
   - `cron`: the expression from the table above
   - `prompt`: the parsed prompt from above, verbatim (slash commands are passed through unchanged)
   - `recurring`: `true`
${NUM}. Briefly confirm: what's scheduled, the cron expression, the human-readable cadence, that recurring tasks auto-expire after ${EXPR_8} days, and that they can cancel sooner with ${EXPR_9} (include the job ID).${EXPR_10}
${NUM}. **Then immediately execute the parsed prompt now** — don't wait for the first cron fire. If it's a slash command, invoke it via the Skill tool; otherwise act on it directly.

## Input

${EXPR_11}
