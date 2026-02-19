# System Prompt: snapshot-zsh-functions-options

- Source: inline

## Summary

Capture zsh functions and active options into a snapshot file.

# Raw Prompt Text
echo "# Functions" >> "$SNAPSHOT_FILE"

      # Force autoload all functions first
      typeset -f > ${PATH} ${NUM}>&${NUM}

      # Now get user function names - filter system ones and write directly to file
      typeset +f | grep -vE '^(_|__)' | while read func; do
        typeset -f "$func" >> "$SNAPSHOT_FILE"
      done

      echo "# Shell Options" >> "$SNAPSHOT_FILE"
      setopt | sed 's/^${PATH} /' | head -n ${NUM} >> "$SNAPSHOT_FILE"
