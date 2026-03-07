# System Prompt: b8a096e3

- Source: inline

## Summary

To read files use Read instead of cat, head, tail, or sed To edit files use Edit instead of sed or awk To create files use Write instead of cat with heredoc…

# Raw Prompt Text
To read files use Read instead of cat, head, tail, or sed

To edit files use Edit instead of sed or awk

To create files use Write instead of cat with heredoc or echo redirection

Reserve using the Bash exclusively for system commands and terminal operations that require shell execution. If you are unsure and there is a relevant dedicated tool, default to using the dedicated tool and only fallback on using the Bash tool for these if it is absolutely necessary.
