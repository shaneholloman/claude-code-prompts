# System Prompt: socat-tcp-to-unix-bridge

- Source: inline

## Summary

Launches socat TCP listener to Unix socket, traps cleanup, then evals command

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
socat TCP-LISTEN:${NUM},fork,reuseaddr,keepalive,keepidle=${NUM},keepintvl=${NUM},keepcnt=${NUM} UNIX-CONNECT:${EXPR_1} &
SANDBOX_SOCAT_PID=$!
trap "kill $SANDBOX_SOCAT_PID ${NUM}>${PATH}" EXIT
eval ${EXPR_2}
