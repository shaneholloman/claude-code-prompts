# System Prompt: check-rg-and-alias

- Source: inline

## Summary

Append snapshot logic to check for rg command and define a fallback alias.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | fallback command string used for the rg alias | None |

# Raw Prompt Text
# Check for rg availability
      echo "# Check for rg availability" >> "$SNAPSHOT_FILE"
      echo "if ! command -v rg >${PATH} ${NUM}>&${NUM}; then" >> "$SNAPSHOT_FILE"
      echo '  alias rg='"'${EXPR_1}
