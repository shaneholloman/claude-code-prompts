# System Prompt: default-ops-no-network

- Source: inline

## Summary

Default-allow policy denying all network except localhost proxy bind/inbound/outbound ports.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
(version ${NUM})
;; Allow all operations by default except network
(allow default)

;; Deny all network operations
(deny network*)

;; Allow localhost TCP operations for the HTTP proxy
(allow network-bind (local ip "localhost:${EXPR_1}"))
(allow network-inbound (local ip "localhost:${EXPR_2}"))
(allow network-outbound (remote ip "localhost:${EXPR_3}"))
