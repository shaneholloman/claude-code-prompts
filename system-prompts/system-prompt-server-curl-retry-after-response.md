# System Prompt: server-curl-retry-after-response

- Source: native-reference-match

## Summary

Verifying server changes with curl and response handling.

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
# System Prompt: server-curl-retry-after-response

- Source: inline

## Summary

Verifying server changes with curl and response handling.

# Raw Prompt Text
# Verifying a server${EXPR_1} change

The handle is `curl` (or equivalent). The evidence is the response.

## Pattern

${EXPR_2}. Start the server (background, with a readiness poll — see below)
${EXPR_3}. `curl` the route the diff touches, with inputs that hit the changed branch
${EXPR_4}. Capture the full response (status + headers + body)
${EXPR_5}. Compare to expected

## Lifecycle

If there's a run-skill it handles this. If not:

```bash
<start-command> &> ${EXPR_6} &
SERVER_PID=$!
for i in {${EXPR_7}..${EXPR_8}}; do curl -sf localhost:PORT${EXPR_9} >${EXPR_10} && break; sleep ${EXPR_11}; done
# ... your curls ...
kill $SERVER_PID
```

No readiness endpoint? Poll the route you're about to test until it
stops returning connection-refused, then add a beat.

## Worked example

**Diff:** adds a `Retry-After` header to ${EXPR_12} responses in `rateLimit.ts`.
**Claim (PR body):** "clients can now back off correctly."

**Inference:** hitting the rate limit should now return `Retry-After: <n>`
in the response headers. It didn't before.

**Plan:**
${EXPR_13}. Start server
${EXPR_14}. Hit the rate-limited endpoint enough times to trigger ${EXPR_15}
${EXPR_16}. Check the ${EXPR_17} response has `Retry-After` header
${EXPR_18}. Check the value is a positive integer

**Execute:**
```bash
# trigger the limit — ${EXPR_19} fast requests, limit is ${EXPR_20}${EXPR_21} per the diff
for i in {${EXPR_22}..${EXPR_23}}; do curl -s -o ${EXPR_24} -w "%{http_code}\n" localhost:${EXPR_25}${EXPR_26}; done
# → ${EXPR_27} ${EXPR_28} ${EXPR_29} ${EXPR_30} ${EXPR_31} ${EXPR_32} ${EXPR_33} ${EXPR_34} ${EXPR_35} ${EXPR_36}

# capture the ${EXPR_37} headers
curl -si localhost:${EXPR_38}${EXPR_39} | head -${EXPR_40}
# → HTTP${EXPR_41} ${EXPR_42} Too Many Requests
# → Retry-After: ${EXPR_43}
# → ...
```

**Verdict:** PASS — `Retry-After: ${EXPR_44}` present, positive integer.

## What FAIL looks like

- Header absent → the diff didn't take effect, or you're not actually
  hitting the ${EXPR_45} path (check the status code first)
- Header present but value is `NaN` / `undefined` / negative → the
  logic is wrong
- You got 200s all the way through → you never triggered the changed
  path. Tighten the request burst or check the rate limit config.
