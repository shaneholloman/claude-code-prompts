# System Data Block: repo-file-put-update-3

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

${EXPR_6}

${EXPR_7}

${EXPR_8}

${EXPR_9}

${EXPR_10}

userSettings

projectSettings

localSettings

Task ${EXPR_11}

(type: ${EXPR_12})

(status: ${EXPR_13})

(description: ${EXPR_14})

Task #${EXPR_15}: ${EXPR_16}

Status: ${EXPR_17}

Description: ${EXPR_18}

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

${EXPR_19}

${EXPR_20}

${EXPR_21}

${EXPR_22}

${EXPR_23}

${EXPR_24}

${EXPR_25}

${EXPR_26}

${EXPR_27}

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

repos/${EXPR_28}${PATH}${EXPR_29}

-f

message="Update ${EXPR_30}"

-f

content=${EXPR_31}

-f

branch=${EXPR_32}

sentry-trace

${EXPR_33}
