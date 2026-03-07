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
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |

# Raw Prompt Text
unalias find ${NUM}>${PATH} || true
unalias grep ${NUM}>${PATH} || true
function find {
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=bfs ${EXPR_1} ${EXPR_2}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=bfs ${EXPR_3} ${EXPR_4}
  elif [[ $BASHPID != $$ ]]; then
    exec -a bfs ${EXPR_5} ${EXPR_6}
  else
    (exec -a bfs ${EXPR_7} ${EXPR_8})
  fi
}
function grep {
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=ugrep ${EXPR_9} ${EXPR_10}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=ugrep ${EXPR_11} ${EXPR_12}
  elif [[ $BASHPID != $$ ]]; then
    exec -a ugrep ${EXPR_13} ${EXPR_14}
  else
    (exec -a ugrep ${EXPR_15} ${EXPR_16})
  fi
}
