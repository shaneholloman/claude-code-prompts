# System Prompt: socat-tcp-to-unix-forwarding

- Source: inline

## Summary

Launches socat TCP listeners to UNIX sockets, traps exit for cleanup, then runs command.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
socat TCP-LISTEN:${NUM},fork,reuseaddr UNIX-CONNECT:${EXPR_1} >${PATH} ${NUM}>&${NUM} &
socat TCP-LISTEN:${NUM},fork,reuseaddr UNIX-CONNECT:${EXPR_2} >${PATH} ${NUM}>&${NUM} &
trap "kill %${NUM} %${NUM} ${NUM}>${PATH}; exit" EXIT
eval ${EXPR_3}
