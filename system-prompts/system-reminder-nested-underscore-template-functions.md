# System Reminder: nested-underscore-template-functions

- Source: inline

## Summary

Nested compiled template functions that concatenate output into a string buffer.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |

# Raw Prompt Text
function(${EXPR_1}) {
obj || (obj = {});
var __t, __p = '', __e = _.escape, __j = Array.prototype.join;
function print() { __p += __j.call(arguments, '') }
function(${EXPR_2}) {
obj || (obj = {});
var __t, __p = '', __e = _.escape, __j = Array.prototype.join;
function print() { __p += __j.call(arguments, '') }
${EXPR_3}return __p
}return __p
}
