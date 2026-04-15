# System Reminder: memory-snapshot-heapdump

- Source: inline

## Summary

Displays memory state details in a heap dump.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
[HeapDump] Memory state:
  heapUsed: ${EXPR_1} GB (in snapshot)
  external: ${EXPR_2} GB (NOT in snapshot)
  rss: ${EXPR_3} GB (total process)
  ${EXPR_4}
