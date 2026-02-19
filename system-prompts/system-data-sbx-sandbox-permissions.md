# System Data Block: sbx-sandbox-permissions

- Source: inline

## Summary

Sandbox profile denies by default with SBX tags, allows core process, IPC, and system access.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
(version ${NUM})

(deny default (with message "SBX_${EXPR_1}"))

; LogTag: SBX_${EXPR_2}

; Essential permissions

(allow process*)

(allow signal)

(allow sysctl-read)

(allow system-socket)

(allow mach*)

(allow ipc*)

(allow iokit*)

(allow user-preference-read)

(allow authorization-right-obtain)

(allow distributed-notification-post)

(allow file-ioctl)
