# System Prompt: ed8e014b

- Source: inline

## Summary

Remote Control - Connect your local environment to claude.ai… USAGE claude remote-control [options] … OPTIONS --name <name> Name for the session (shown in cl…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
Remote Control - Connect your local environment to claude.ai${PATH}

USAGE
  claude remote-control [options]
${EXPR_1}
OPTIONS
  --name <name>                    Name for the session (shown in claude.ai${PATH})
  --permission-mode <mode>         Permission mode for spawned sessions
                                   (${EXPR_2})
  --debug-file <path>              Write debug logs to file
  -v, --verbose                    Enable verbose output
  -h, --help                       Show this help
${EXPR_3}
DESCRIPTION
  Remote Control allows you to control sessions on your local device from
  claude.ai${PATH} (${URL}). Run this command in the
  directory you want to work in, then connect from the Claude app or web.

  The 'server' subcommand runs as a persistent server that accepts multiple
  concurrent sessions without pre-creating an initial session. By default
  all sessions share the current directory. Use --spawn-worktree-sessions
  to give each session its own isolated git worktree.

NOTES
  - You must be logged in with a Claude account that has a subscription
  - Run `claude` first in the directory to accept the workspace trust dialog
  - --spawn-worktree-sessions requires a git repository or WorktreeCreate${PATH} hooks
