# System Data Block: cli-linters-metadata-4

- Source: inline

## Summary

Defines Claude Code CLI role, enumerates linter tools, and logs background bash command status.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | Task | None |
| `EXPR_2` | Bash | None |
| `EXPR_3` | Glob | None |
| `EXPR_4` | Grep | None |
| `EXPR_5` | ExitPlanMode | None |
| `EXPR_6` | Read | None |
| `EXPR_7` | Edit | None |
| `EXPR_8` | MultiEdit | None |
| `EXPR_9` | Write | None |
| `EXPR_10` | NotebookEdit | None |
| `EXPR_11` | WebFetch | None |
| `EXPR_12` | WebSearch | None |
| `EXPR_13` | BashOutput | None |
| `EXPR_14` | KillShell | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
${EXPR_1: 'Task'}

${EXPR_2: 'Bash'}

${EXPR_3: 'Glob'}

${EXPR_4: 'Grep'}

${EXPR_5: 'ExitPlanMode'}

${EXPR_6: 'Read'}

${EXPR_7: 'Edit'}

${EXPR_8: 'MultiEdit'}

${EXPR_9: 'Write'}

${EXPR_10: 'NotebookEdit'}

${EXPR_11: 'WebFetch'}

${EXPR_12: 'WebSearch'}

${EXPR_13: 'BashOutput'}

${EXPR_14: 'KillShell'}

You are Claude Code, Anthropic's official CLI for Claude.

eslint

eslint-plugin

tslint

prettier

stylelint

jshint

standardjs

xo

rome

biome

deno-lint

rubocop

pylint

flake8

black

ruff

clippy

rustfmt

golangci-lint

gofmt

swiftlint

detekt

ktlint

checkstyle

pmd

sonarqube

sonarjs

Background Bash ${EXPR_15}

(command: ${EXPR_16})

(status: ${EXPR_17})
