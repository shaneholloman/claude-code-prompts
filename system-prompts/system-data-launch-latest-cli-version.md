# System Data Block: launch-latest-cli-version

- Source: inline

## Summary

Launcher script selects latest executable CLI via symlink or newest version directory.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
#!${PATH}

# Claude CLI Launcher Script

# Set terminal title
printf '\${NUM}]${NUM};claude\${NUM}'

# XDG-based locations
VERSIONS_DIR="${EXPR_1}"
LATEST_LINK="${EXPR_2}${PATH}"

# Try to run the latest symlink if it exists
if [[ -L "$LATEST_LINK" ]] && [[ -x "$LATEST_LINK" ]]; then
    exec "$LATEST_LINK" "$@"
fi

# If latest doesn't exist or failed to execute, try versions by modification time
if [[ -d "$VERSIONS_DIR" ]]; then
    # Use ls -t to sort by modification time (newest first)
    # Filter for executable files only
    for VERSION_FILE in $(ls -t "$VERSIONS_DIR" ${NUM}>${PATH}); do
        FULL_PATH="$VERSIONS_DIR/$VERSION_FILE"
        if [[ -f "$FULL_PATH" ]] && [[ -x "$FULL_PATH" ]]; then
            exec "$FULL_PATH" "$@"
        fi
    done
fi

# No binary found
echo "Error: No Claude CLI binary found." >&${NUM}
echo "Looked for:" >&${NUM}
echo "  Latest symlink: $LATEST_LINK" >&${NUM}
echo "  Versions directory: $VERSIONS_DIR" >&${NUM}
exit ${NUM}
