# System Prompt: fix-cli-executable-name

- Source: inline

## Summary

Fixes missing "global" executable by revising command description usage or executableFile setting.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
'global' does not exist
 - if '${EXPR_1}' is not meant to be an executable command, remove description parameter from '.command()' and use '.description()' instead
 - if the default executable name is not suitable, use the executableFile option to supply a custom name or path
 - local
