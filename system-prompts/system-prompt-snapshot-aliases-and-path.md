# System Prompt: snapshot-aliases-and-path

- Source: inline

## Summary

Write a shell snapshot file that unaliases, captures aliases, and exports PATH.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
SNAPSHOT_FILE=${EXPR_1}
      source "${EXPR_2}" < ${PATH}

      # First, create${PATH} the snapshot file
      echo "# Snapshot file" >| $SNAPSHOT_FILE

      # When this file is sourced, we first unalias to avoid conflicts
      # This is necessary because aliases get "frozen" inside function definitions at definition time,
      # which can cause unexpected behavior when functions use commands that conflict with aliases
      echo "# Unset all aliases to avoid conflicts with functions" >> $SNAPSHOT_FILE
      echo "unalias -a ${NUM}>${PATH} || true" >> $SNAPSHOT_FILE

      local

      echo "# Aliases" >> $SNAPSHOT_FILE
      alias | sed 's/^alias //g' | sed 's/^${PATH} -- /' | head -n ${NUM} >> $SNAPSHOT_FILE

      # Add PATH to the file
      echo "export PATH='${EXPR_3}'" >> $SNAPSHOT_FILE
