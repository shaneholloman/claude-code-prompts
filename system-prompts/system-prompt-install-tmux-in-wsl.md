# System Prompt: bff8d62b

- Source: inline

## Summary

Explains installing WSL and tmux and starting a tmux session for swarms.

# Raw Prompt Text
To use agent swarms, you need tmux which requires WSL (Windows Subsystem for Linux).
Install WSL first, then inside WSL run:
  sudo apt install tmux
Then start a tmux session with: tmux new-session -s claude
