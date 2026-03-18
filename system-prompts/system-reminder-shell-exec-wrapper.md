# System Prompt: shell-exec-wrapper

- Source: inline

## Summary

Shebang-based wrapper execs a computed target path, forwarding all command-line arguments.

# Raw Prompt Text
#!${PATH}
exec "${EXPR_1}${PATH}" "$@"
