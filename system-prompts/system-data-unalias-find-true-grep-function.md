# System Data Block: 74d4453c

- Source: inline

## Summary

unalias find …>… || true unalias grep …>… || true function find { if [[ -n $ZSH_VERSION ]]; then ARGV0=bfs … … elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE"…

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

# Raw Prompt Text
unalias find ${NUM}>${PATH} || true
unalias grep ${NUM}>${PATH} || true
function find {
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=bfs ${EXPR_1} ${NUM}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=bfs ${EXPR_2} ${NUM}
  elif [[ $BASHPID != $$ ]]; then
    exec -a bfs ${EXPR_3} ${NUM}
  else
    (exec -a bfs ${EXPR_4} ${NUM})
  fi
}
function grep {
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=ugrep ${EXPR_5} ${NUM}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=ugrep ${EXPR_6} ${NUM}
  elif [[ $BASHPID != $$ ]]; then
    exec -a ugrep ${EXPR_7} ${NUM}
  else
    (exec -a ugrep ${EXPR_8} ${NUM})
  fi
}
