# System Reminder: template-return-function-escape

- Source: inline

## Summary

Escape-enabled template function building output string from object and print calls.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
${EXPR_1}return function(${EXPR_2}) {
obj || (obj = {});
var __t, __p = '', __e = _.escape, __j = Array.prototype.join;
function print() { __p += __j.call(arguments, '') }
${EXPR_3}return __p
}
