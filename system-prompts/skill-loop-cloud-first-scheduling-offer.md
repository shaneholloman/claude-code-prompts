# Skill: loop-cloud-first-scheduling-offer

- Source: native-reference-match

## Summary

Check conditions before scheduling tasks.

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
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
# Skill: loop-cloud-first-scheduling-offer

- Source: native-reference-match

## Summary

Check conditions before scheduling tasks.

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
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
# Skill: loop-cloud-first-scheduling-offer

- Source: native-reference-match

## Summary

Check conditions before scheduling tasks.

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
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
# Skill: loop-cloud-first-scheduling-offer

- Source: native-reference-match

## Summary

Offer cloud first Before any scheduling step, check whether EITHER is true: - the parsed interval (rule … or …) is **≥… minutes**, or - regardless of which r…

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

# Raw Prompt Text
## Offer cloud first

Before any scheduling step, check whether EITHER is true:
- the parsed interval (rule ${EXPR_1} or ${EXPR_2}) is **≥${EXPR_3} minutes**, or
- regardless of which rule matched, the original input uses daily phrasing ("every morning", "daily", "every day", "each night", "every weekday")

If either is true, call ${EXPR_4} first:
- `question`: "This loop stops when you close this session. Set it up as a cloud schedule instead so it keeps running?"
- `header`: "Schedule"
- `options`: `[{label: "Cloud schedule (recommended)", description: "Runs in Anthropic's cloud even after you close this session"}, {label: "This session only", description: "Runs in this terminal until you exit"}]`

If they pick **Cloud schedule**: do NOT call ${EXPR_5}. Invoke the `schedule` skill directly via the ${EXPR_6} tool with `args` set to their original input verbatim (e.g. `${EXPR_7}({skill: "schedule", args: "every morning tell me a joke"})`), then follow that skill's instructions to completion. Do NOT tell the user to run ${EXPR_8} themselves. **Then stop — do not continue to any section below** (no ${EXPR_9}, no ${EXPR_10}, no "execute the prompt now").
If they pick **This session only**:
- If the trigger was a parsed ≥${EXPR_11}-minute interval (rule ${EXPR_12} or ${EXPR_13}): continue below with that interval.
- If the trigger was daily phrasing only (rule ${EXPR_14}, no parsed interval): do NOT call ${EXPR_15}. Explain that a daily-cadence loop won't fire before this session closes, so there's nothing useful to schedule locally — suggest they either pick Cloud schedule, or re-run `${EXPR_16}` with an explicit shorter interval (e.g. `${EXPR_17} 1h <prompt>`) if they want a session loop. Then stop.
If neither trigger condition was met: continue below.
