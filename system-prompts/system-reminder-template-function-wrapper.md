# System Reminder: template-function-wrapper

- Source: inline

## Summary

Underscore-style template wrapper using object scope, escaping, print join, and output buffer.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
with (obj) {
function(${EXPR_1}) {
obj || (obj = {});
var __t, __p = '', __e = _.escape, __j = Array.prototype.join;
function print() { __p += __j.call(arguments, '') }
${EXPR_2}return __p
}
}
