# System Data Block: put-repo-update-linter-metadata-2

- Source: inline

## Summary

GitHub API PUT updates repository file with commit message, content, branch, and linter error schema.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |

# Raw Prompt Text
api

--method

PUT

repos/${EXPR_1}${PATH}${EXPR_2}

-f

message="Update ${EXPR_3}"

-f

content=${EXPR_4}

-f

branch=${EXPR_5}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

${NUM}

name

message

stack

line

column

fileName

lineNumber

columnNumber

toJSON

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

asDouble

asInt

${EXPR_6}

Found ${EXPR_7} symbols in workspace:

${EXPR_8}

${EXPR_9}

${EXPR_10}

${EXPR_11}
