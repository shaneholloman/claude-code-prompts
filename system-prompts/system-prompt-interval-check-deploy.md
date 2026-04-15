# System Prompt: interval-check-deploy


## Summary

Multiple prompts (2)

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Usage: ${PATH} [interval] <prompt>

Run a prompt or slash command on a recurring interval — or with no interval, let the model self-pace based on the task.

Intervals: Ns, Nm, Nh, Nd (e.g. 5m, 30m, 2h, 1d). Minimum granularity is ${NUM} minute.
If no interval is specified, the model picks a delay between iterations based on what it's doing.

Examples:
  ${PATH} 5m ${PATH}
  ${PATH} 30m check the deploy
  ${PATH} 1h ${PATH} ${NUM}
  ${PATH} check the deploy          (dynamic — model picks delays)
  ${PATH} check the deploy every 20m${EXPR_1}
