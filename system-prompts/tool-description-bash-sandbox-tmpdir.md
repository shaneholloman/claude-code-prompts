# Tool Description: bash-sandbox-tmpdir

- Source: native-reference-match

## Summary

For temporary files, always use the `$TMPDIR` environment variable.

# Raw Prompt Text
For temporary files, always use the `$TMPDIR` environment variable. TMPDIR is automatically set to the correct sandbox-writable directory in sandbox mode. Do NOT use `${PATH}` directly - use `$TMPDIR` instead.
