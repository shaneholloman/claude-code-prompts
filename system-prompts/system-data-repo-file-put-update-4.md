# System Data Block: repo-file-put-update-4

- Source: inline

## Summary

Template for updating repository file contents via API PUT with task metadata and JSON Schema keywords.

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
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |
| `EXPR_18` | None | None |
| `EXPR_19` | None | None |
| `EXPR_20` | None | None |
| `EXPR_21` | None | None |
| `EXPR_22` | None | None |
| `EXPR_23` | None | None |
| `EXPR_24` | None | None |

# Raw Prompt Text
${EXPR_1}

${EXPR_2}

${EXPR_3}

${EXPR_4}

${EXPR_5}

userSettings

projectSettings

localSettings

Task ${EXPR_6}

(type: ${EXPR_7})

(status: ${EXPR_8})

(description: ${EXPR_9})

Task #${EXPR_10}: ${EXPR_11}

Status: ${EXPR_12}

Description: ${EXPR_13}

$schema

$id

id

$data

$async

title

description

default

definitions

examples

readOnly

writeOnly

contentMediaType

contentEncoding

additionalItems

then

else

number

integer

string

array

object

boolean

null

$schema

$id

id

$data

$async

title

description

default

definitions

examples

readOnly

writeOnly

contentMediaType

contentEncoding

additionalItems

then

else

number

integer

string

array

object

boolean

null

${PATH}

${PATH}

${PATH}

${PATH}

${EXPR_14}

${EXPR_15}

${EXPR_16}

${EXPR_17}

${EXPR_18}

${EXPR_19}

${EXPR_20}

${EXPR_21}

${EXPR_22}

$schema

$id

id

$data

$async

title

description

default

definitions

examples

readOnly

writeOnly

contentMediaType

contentEncoding

additionalItems

then

else

number

integer

string

array

object

boolean

null

$schema

$id

id

$data

$async

title

description

default

definitions

examples

readOnly

writeOnly

contentMediaType

contentEncoding

additionalItems

then

else

number

integer

string

array

object

boolean

null

$schema

$id

id

$data

$async

title

description

default

definitions

examples

readOnly

writeOnly

contentMediaType

contentEncoding

additionalItems

then

else

number

integer

string

array

object

boolean

null

api

--method

PUT

repos/${EXPR_23}${PATH}${EXPR_24}

-f

message="Update ${EXPR_25}"

-f

content=${EXPR_26}

-f

branch=${EXPR_27}
