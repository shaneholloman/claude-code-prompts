# System Data Block: write-conversation-title-2

- Source: inline

## Summary

Requests a fixed-length conversation title, returning only the title text.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Claude Code | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
Please write a ${NUM}-${NUM} word title the following conversation:

${EXPR_1}


Respond with the title for the conversation and nothing else.

You are ${EXPR_2: 'Claude Code'}, Anthropic's official CLI for Claude.

${NUM}

${NUM}

${NUM}

${NUM}

${EXPR_3}

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
