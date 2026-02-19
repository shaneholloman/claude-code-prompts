# System Prompt: add-native-path-export

- Source: inline

## Summary

Appends export PATH with $HOME… into shell profile and reloads it

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Native installation exists but ~${PATH} is not in your PATH. Run:

echo 'export PATH="$HOME${PATH}:$PATH"' >> ${EXPR_1} && source ${EXPR_2}
