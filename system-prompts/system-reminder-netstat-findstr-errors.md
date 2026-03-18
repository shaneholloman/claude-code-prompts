# System Prompt: netstat-findstr-errors

- Source: inline

## Summary

Check netstat for loaded errors.

# Raw Prompt Text
netstat -ano | findstr :${EXPR_1} loaded with errors
