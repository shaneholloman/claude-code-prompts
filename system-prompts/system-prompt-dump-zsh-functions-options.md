# System Prompt: dump-zsh-functions-options

- Source: inline

## Summary

Print loaded zsh functions and current setopt options.

# Raw Prompt Text
echo "# Functions"
      # Force autoload all functions first
      typeset -f > ${PATH} ${NUM}>&${NUM}
      # Now get user function names - filter system ones
      typeset +f | grep -vE '^(_|__)' | while read func; do
        typeset -f "$func"
      done

      echo "# Shell Options"
      setopt | sed 's/^${PATH} /' | head -n ${NUM}
