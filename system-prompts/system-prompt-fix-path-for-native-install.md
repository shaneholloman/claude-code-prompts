# System Prompt: fix-path-for-native-install

- Source: inline

## Summary

Adds a native install directory to PATH via an export line appended to a file.

# Raw Prompt Text
Native installation exists but ~${PATH} is not in your PATH. Run:

echo 'export PATH="$HOME${PATH}:$PATH"' >> stdio && source stdio
