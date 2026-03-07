# System Data Block: 4dbf194c

- Source: inline

## Summary

function … { if [[ -n $ZSH_VERSION ]]; then ARGV0=… … … elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then ARG…

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
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |

# Raw Prompt Text
function ${EXPR_1} {
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=${EXPR_2} ${EXPR_3} ${EXPR_4}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=${EXPR_5} ${EXPR_6} ${EXPR_7}
  elif [[ $BASHPID != $$ ]]; then
    exec -a ${EXPR_8} ${EXPR_9} ${EXPR_10}
  else
    (exec -a ${EXPR_11} ${EXPR_12} ${EXPR_13})
  fi
}
