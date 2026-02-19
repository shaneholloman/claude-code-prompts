# System Prompt: add-native-path-export

- Source: inline

## Summary

Appends export PATH with $HOME… into shell profile and reloads it

# Raw Prompt Text
Native installation exists but ~${PATH} is not in your PATH. Run:

echo 'export PATH="$HOME${PATH}:$PATH"' >> ${NUM} && source ${NUM}
