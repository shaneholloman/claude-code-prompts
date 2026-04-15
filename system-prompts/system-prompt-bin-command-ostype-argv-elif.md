# System Data Block: function-command-ostype-argv

- Source: inline

## Summary

Function to execute commands based on conditions.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |

# Raw Prompt Text
function ${EXPR_1} {
  local _cc_bin="${EXPR_2}"
  [[ -x $_cc_bin ]] || _cc_bin=$(command -v claude ${NUM}>${PATH})
  if [[ ! -x $_cc_bin ]]; then command ${EXPR_3} "$@"; return; fi
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=${EXPR_4} "$_cc_bin" ${EXPR_5}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=${EXPR_6} "$_cc_bin" ${EXPR_7}
  elif [[ $BASHPID != $$ ]]; then
    exec -a ${EXPR_8} "$_cc_bin" ${EXPR_9}
  else
    (exec -a ${EXPR_10} "$_cc_bin" ${EXPR_11})
  fi
}
