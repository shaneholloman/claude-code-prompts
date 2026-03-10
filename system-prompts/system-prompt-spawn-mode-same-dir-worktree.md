# System Prompt: 3ab70381

- Source: inline

## Summary

--spawn <mode> Spawn mode: same-dir, worktree, session (default: same-dir) --capacity <N> Max concurrent sessions in worktree or same-dir mode (default: …) -…

# Raw Prompt Text
--spawn <mode>                   Spawn mode: same-dir, worktree, session
                                   (default: same-dir)
  --capacity <N>                   Max concurrent sessions in worktree or
                                   same-dir mode (default: ${NUM})
  --[no-]create-session-in-dir     Pre-create a session in the current
                                   directory; in worktree mode this session
                                   stays in cwd while on-demand sessions get
                                   isolated worktrees (default: on)
