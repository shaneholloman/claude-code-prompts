# System Data Block: write-alias-path-snapshot

- Source: inline

## Summary

Save current aliases and PATH export into a snapshot file for sourcing later.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
SNAPSHOT_FILE=${EXPR_1}
      source "${EXPR_2}" < ${PATH}
      {
      local

      echo "# Aliases"
      alias | sed 's/^alias //g' | sed 's/^${PATH} -- /' | head -n ${NUM}
      echo "export PATH='${EXPR_3}'"
      } >| $SNAPSHOT_FILE
