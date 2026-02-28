# System Prompt: 5bd1a0df

- Source: inline

## Summary

Remote Control - Connect your local environment to claude.ai… USAGE claude remote-control [options] OPTIONS --permission-mode <mode> Permission mode for spaw…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |

# Raw Prompt Text
Remote Control - Connect your local environment to claude.ai${PATH}

USAGE
  claude remote-control [options]

OPTIONS
  --permission-mode <mode>  Permission mode for spawned sessions
                            (${EXPR_1})
  --debug-file <path>       Write debug logs to file
  -v, --verbose             Enable verbose output
  -h, --help                Show this help

DESCRIPTION
  Remote Control allows you to control sessions on your local device from
  claude.ai${PATH} (${URL}). Run this command in the
  directory you want to work in, then connect from the Claude app or web.

NOTES
  - You must be logged in with a Claude account that has a subscription
  - Run `claude` first in the directory to accept the workspace trust dialog
