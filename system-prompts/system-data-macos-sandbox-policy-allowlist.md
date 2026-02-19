# System Data Block: macos-sandbox-policy-allowlist

- Source: inline

## Summary

macOS sandbox profile allowing core process actions, specific Mach services, and IPC primitives

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
(version ${NUM})

(deny default (with message "${EXPR_1}"))

; LogTag: ${EXPR_2}

; Essential permissions - based on Chrome sandbox policy

; Process permissions

(allow process-exec)

(allow process-fork)

(allow process-info* (target same-sandbox))

(allow signal (target same-sandbox))

; User preferences

(allow user-preference-read)

; Mach IPC - specific services only (no wildcard)

(allow mach-lookup

  (global-name "com.apple.audio.systemsoundserver")

  (global-name "com.apple.distributed_notifications@Uv3")

  (global-name "com.apple.FontObjectsServer")

  (global-name "com.apple.fonts")

  (global-name "com.apple.logd")

  (global-name "com.apple.lsd.mapdb")

  (global-name "com.apple.PowerManagement.control")

  (global-name "com.apple.system.logger")

  (global-name "com.apple.system.notification_center")

  (global-name "com.apple.system.opendirectoryd.libinfo")

)

; POSIX IPC - shared memory

(allow ipc-posix-shm)

; POSIX IPC - semaphores for Python multiprocessing

(allow ipc-posix-sem)

; IOKit - specific operations only

(allow iokit-open

  (iokit-registry-entry-class "IOSurfaceRootUserClient")

  (iokit-registry-entry-class "RootDomainUserClient")

  (iokit-user-client-class "IOSurfaceSendRight")

)

; IOKit properties

(allow iokit-get-properties)

; sysctl - specific sysctls only

(allow sysctl-read

  (sysctl-name "hw.activecpu")

  (sysctl-name "hw.busfrequency_compat")

  (sysctl-name "hw.byteorder")

  (sysctl-name "hw.cacheconfig")

  (sysctl-name "hw.cachelinesize_compat")

  (sysctl-name "hw.cpufamily")

  (sysctl-name "hw.cpufrequency_compat")

  (sysctl-name "hw.cputype")

  (sysctl-name "hw.l1dcachesize_compat")

  (sysctl-name "hw.l1icachesize_compat")

  (sysctl-name "hw.l2cachesize_compat")

  (sysctl-name "hw.l3cachesize_compat")

  (sysctl-name "hw.logicalcpu")

  (sysctl-name "hw.logicalcpu_max")

  (sysctl-name "hw.machine")

  (sysctl-name "hw.memsize")

  (sysctl-name "hw.ncpu")

  (sysctl-name "hw.nperflevels")

  (sysctl-name "hw.packages")

  (sysctl-name "hw.pagesize_compat")

  (sysctl-name "hw.pagesize")

  (sysctl-name "hw.physicalcpu_max")

  (sysctl-name "hw.tbfrequency_compat")

  (sysctl-name "hw.vectorunit")

  (sysctl-name "kern.argmax")

  (sysctl-name "kern.bootargs")

  (sysctl-name "kern.hostname")

  (sysctl-name "kern.maxfiles")

  (sysctl-name "kern.maxfilesperproc")

  (sysctl-name "kern.maxproc")

  (sysctl-name "kern.ngroups")

  (sysctl-name "kern.osproductversion")

  (sysctl-name "kern.osrelease")

  (sysctl-name "kern.ostype")

  (sysctl-name "kern.osvariant_status")

  (sysctl-name "kern.osversion")

  (sysctl-name "kern.secure_kernel")

  (sysctl-name "kern.tcsm_available")

  (sysctl-name "kern.tcsm_enable")

  (sysctl-name "kern.usrstack64")

  (sysctl-name "kern.version")

  (sysctl-name "kern.willshutdown")

  (sysctl-name "security.mac.lockdown_mode_state")

  (sysctl-name "sysctl.proc_cputype")

  (sysctl-name "vm.loadavg")

  (sysctl-name-prefix "hw.optional.arm")

  (sysctl-name-prefix "hw.optional.arm.")

  (sysctl-name-prefix "hw.optional.armv8_")

  (sysctl-name-prefix "hw.perflevel")

  (sysctl-name-prefix "kern.proc.pgrp.")

  (sysctl-name-prefix "kern.proc.pid.")

  (sysctl-name-prefix "net.routetable.")

)

; V8 thread calculations

(allow sysctl-write

  (sysctl-name "kern.tcsm_enable")

)

; Distributed notifications

(allow distributed-notification-post)

; File I/O on device files

(allow file-ioctl (literal "${PATH}"))

(allow file-ioctl (literal "${PATH}"))

(allow file-ioctl (literal "${PATH}"))

(allow file-ioctl (literal "${PATH}"))

(allow file-ioctl (literal "${PATH}"))

(allow file-ioctl (literal "${PATH}"))

(allow file-ioctl file-read-data file-write-data

  (require-all

    (literal "${PATH}")

    (vnode-type CHARACTER-DEVICE)

  )

)
