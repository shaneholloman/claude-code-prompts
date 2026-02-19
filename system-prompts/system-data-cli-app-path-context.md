# System Data Block: cli-app-path-context

- Source: inline

## Summary

Sets Claude CLI identity, lists terminal color styles, and defines app/… path template.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Claude Code | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
You are ${EXPR_1: 'Claude Code'}, Anthropic's official CLI for Claude.

${NUM}

${NUM}

${NUM}

${NUM}

${EXPR_2}

underline

inverse

grey

yellow

red

green

blue

white

cyan

magenta

brightYellow

brightRed

brightGreen

brightBlue

brightWhite

brightCyan

brightMagenta

app/${EXPR_3}
