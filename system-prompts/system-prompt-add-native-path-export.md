# System Prompt: add-native-path-export

- Source: inline

## Summary

Appends export PATH with $HOME… into shell profile and reloads it

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
Native installation exists but ~${PATH} is not in your PATH. Run:

echo 'export PATH="$HOME${PATH}:$PATH"' >> mcp__${EXPR_1}__${EXPR_2} && source mcp__${EXPR_3}__${EXPR_4}
