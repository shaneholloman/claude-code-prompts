# System Prompt: snapshot-functions-typeset-dump

- Source: inline

## Summary

Captures user function definitions via typeset and writes them directly to the snapshot.

# Raw Prompt Text
echo "# Functions" >> "$SNAPSHOT_FILE"

      # Force autoload all functions first
      typeset -f > ${PATH} ${NUM}>&${NUM}

      # Now get user function names - filter system ones and write directly to file
      typeset +f | grep -vE '^(_|__)' | while read func; do
        typeset -f "$func" >> "$SNAPSHOT_FILE"
      done
