# System Prompt: socat-tcp-to-unix-bridge-2

- Source: inline

## Summary

Start socat TCP listeners forwarding to a UNIX socket, with exit cleanup trap.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
socat TCP-LISTEN:${NUM},fork,reuseaddr UNIX-CONNECT:${PATH} >${PATH} ${NUM}>&${NUM} &

socat TCP-LISTEN:${NUM},fork,reuseaddr UNIX-CONNECT:${EXPR_1} >${PATH} ${NUM}>&${NUM} &

trap "kill %${NUM} %${NUM} ${NUM}>${PATH}; exit" EXIT
