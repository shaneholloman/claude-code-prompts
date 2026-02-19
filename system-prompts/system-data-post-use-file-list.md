# System Data Block: post-use-file-list

- Source: inline

## Summary

Post-tool hook listing linters with bash background, command, status, and file paths.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
<post-tool-use-hook>You are Claude Code, Anthropic's official CLI for Claude.

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

Background Bash ${EXPR_1}

(command: ${EXPR_2})

(status: ${EXPR_3})

files<${PATH}>
