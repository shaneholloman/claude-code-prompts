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

# Raw Prompt Text
function ${EXPR_1} {
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=${EXPR_2} ${EXPR_3} ${NUM}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=${EXPR_4} ${EXPR_5} ${NUM}
  elif [[ $BASHPID != $$ ]]; then
    exec -a ${EXPR_6} ${EXPR_7} ${NUM}
  else
    (exec -a ${EXPR_8} ${EXPR_9} ${NUM})
  fi
}
