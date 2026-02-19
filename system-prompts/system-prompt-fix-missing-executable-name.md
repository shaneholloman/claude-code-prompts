# System Prompt: fix-missing-executable-name

- Source: inline

## Summary

Advise fixes when a specified CLI subcommand executable path is missing.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
'${EXPR_1}' does not exist
 - if '${EXPR_2}' is not meant to be an executable command, remove description parameter from '.command()' and use '.description()' instead
 - if the default executable name is not suitable, use the executableFile option to supply a custom name or path
 - ${EXPR_3}
