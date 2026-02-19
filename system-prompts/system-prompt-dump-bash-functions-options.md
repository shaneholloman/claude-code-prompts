# System Prompt: dump-bash-functions-options

- Source: inline

## Summary

Print loaded bash functions and enabled shell options.

# Raw Prompt Text
echo "# Functions"
      # Force autoload all functions first
      declare -f > ${PATH} ${NUM}>&${NUM}
      # Now get user function names - filter system ones
      declare -F | cut -d' ' -f3 | grep -vE '^(_|__)' | while read func; do
        declare -f "$func"
      done

      echo "# Shell Options"
      shopt -p | head -n ${NUM}
      set -o | grep "on" | awk '{print "set -o " $${NUM}}' | head -n ${NUM}
      echo "shopt -s expand_aliases"
