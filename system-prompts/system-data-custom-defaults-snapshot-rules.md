# System Data Block: custom-defaults-snapshot-rules

- Source: inline

## Summary

Snapshot rules replace defaults.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | @anthropic-ai/claude-code | None |
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

# Raw Prompt Text
RSS ${EXPR_1} GB (peak ${EXPR_2} GB) npm view ${EXPR_3: '@anthropic-ai/claude-code'}@${EXPR_4} version
  JS heap        ${EXPR_5}  in snapshot
  array buffers  ${EXPR_6}  not in snapshot
  other external ${EXPR_7}  not in snapshot
  unaccounted    ${EXPR_8}  not in snapshot (code${PATH})
## allow (custom rules replacing defaults)
Custom:
${EXPR_9}

Defaults being replaced:
${EXPR_10}

## soft_deny (custom rules replacing defaults)
Custom:
${EXPR_11}

Defaults being replaced:
${EXPR_12}

## environment (custom rules replacing defaults)
Custom:
${EXPR_13}

Defaults being replaced:
${EXPR_14}
