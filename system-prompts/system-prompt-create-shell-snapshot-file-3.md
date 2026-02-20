# System Prompt: create-shell-snapshot-file-3

- Source: inline

## Summary

Writes a snapshot script file, clears aliases, injects dynamic sections, and verifies output exists

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
SNAPSHOT_FILE=${EXPR_1}
      # No user config file to source

      # First, create${PATH} the snapshot file
      echo "# Snapshot file" >| "$SNAPSHOT_FILE"

      # When this file is sourced, we first unalias to avoid conflicts
      # This is necessary because aliases get "frozen" inside function definitions at definition time,
      # which can cause unexpected behavior when functions use commands that conflict with aliases
      echo "# Unset all aliases to avoid conflicts with functions" >> "$SNAPSHOT_FILE"
      echo "unalias -a ${NUM}>${PATH} || true" >> "$SNAPSHOT_FILE"

      ${EXPR_2}

      ${EXPR_3}

      # Exit silently on success, only report errors
      if [ ! -f "$SNAPSHOT_FILE" ]; then
        echo "Error: Snapshot file was not created at $SNAPSHOT_FILE" >&${NUM}
        exit ${NUM}
      fi
