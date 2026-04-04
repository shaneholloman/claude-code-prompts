# System Prompt: bfs-grep-find-command

- Source: inline

## Summary

Functions for find and grep commands with custom behavior.

# Raw Prompt Text
unalias find ${NUM}>${PATH} || true
unalias grep ${NUM}>${PATH} || true
function find {
  local _cc_bin="${EXPR_1}"
  [[ -x $_cc_bin ]] || _cc_bin=$(command -v claude ${NUM}>${PATH})
  if [[ ! -x $_cc_bin ]]; then command find "$@"; return; fi
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=bfs "$_cc_bin" ${EXPR_2}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=bfs "$_cc_bin" ${EXPR_3}
  elif [[ $BASHPID != $$ ]]; then
    exec -a bfs "$_cc_bin" ${EXPR_4}
  else
    (exec -a bfs "$_cc_bin" ${EXPR_5})
  fi
}
function grep {
  local _cc_bin="${EXPR_6}"
  [[ -x $_cc_bin ]] || _cc_bin=$(command -v claude ${NUM}>${PATH})
  if [[ ! -x $_cc_bin ]]; then command grep "$@"; return; fi
  if [[ -n $ZSH_VERSION ]]; then
    ARGV0=ugrep "$_cc_bin" ${EXPR_7}
  elif [[ "$OSTYPE" == "msys" ]] || [[ "$OSTYPE" == "cygwin" ]] || [[ "$OSTYPE" == "win32" ]]; then
    ARGV0=ugrep "$_cc_bin" ${EXPR_8}
  elif [[ $BASHPID != $$ ]]; then
    exec -a ugrep "$_cc_bin" ${EXPR_9}
  else
    (exec -a ugrep "$_cc_bin" ${EXPR_10})
  fi
}
