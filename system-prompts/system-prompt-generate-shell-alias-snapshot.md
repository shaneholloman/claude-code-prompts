# System Prompt: generate-shell-alias-snapshot

- Source: inline

## Summary

Generate a shell alias snapshot file by unaliasing first, then writing filtered aliases.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |

# Raw Prompt Text
source "${EXPR_1}" < ${PATH} > ${PATH} ${NUM}>&${NUM}

      # First, output snapshot header
      echo "# Snapshot file"

      # When this file is sourced, we first unalias to avoid conflicts
      # This is necessary because aliases get "frozen" inside function definitions at definition time,
      # which can cause unexpected behavior when functions use commands that conflict with aliases
      echo "# Unset all aliases to avoid conflicts with functions"
      echo "unalias -a ${NUM}>${PATH} || true"

      ${EXPR_2}

      echo "# Aliases"
      # Filter out winpty aliases on Windows to avoid "stdin is not a tty" errors
      # Git Bash automatically creates aliases like "alias node='winpty node.exe'" for
      # programs that need Win32 Console in mintty, but winpty fails when there's no TTY
      if [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]]; then
        alias | grep -v "='winpty " | sed 's/^alias //g' | sed 's/^${PATH} -- /' | head -n ${NUM}
      else
        alias | sed 's/^alias //g' | sed 's/^${PATH} -- /' | head -n ${NUM}
      fi

      # Check if rg is available, if not create an alias to bundled ripgrep
      echo "# Check for rg availability"
      echo "if ! command -v rg >${PATH} ${NUM}>&${NUM}; then"
      echo "  alias rg='${EXPR_3}'"
      echo "fi"

      # Add PATH to stdout
      echo "export PATH=${EXPR_4}"
