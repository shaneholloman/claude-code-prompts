# System Data Block: interval-check-deploy

- Source: native-reference-match

## Summary

System Prompt: interval-check-deploy Summary Multiple prompts (…) Placeholder Hints (source-backed) | Expression | Hint | Reference | | --- | --- | --- | | `…

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
# System Prompt: interval-check-deploy


## Summary

Multiple prompts (${NUM})

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Usage: ${EXPR_1} [interval] <prompt>

Run a prompt or slash command on a recurring interval — or with no interval, let the model self-pace based on the task.

Intervals: Ns, Nm, Nh, Nd (e.g. 5m, 30m, 2h, 1d). Minimum granularity is ${EXPR_2} minute.
If no interval is specified, the model picks a delay between iterations based on what it's doing.

Examples:
  ${EXPR_3} 5m ${EXPR_4}
  ${EXPR_5} 30m check the deploy
  ${EXPR_6} 1h ${EXPR_7} ${EXPR_8}
  ${EXPR_9} check the deploy          (dynamic — model picks delays)
  ${EXPR_10} check the deploy every 20m${EXPR_11}
