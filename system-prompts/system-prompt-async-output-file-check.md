# System Prompt: async-output-file-check


## Summary

Announces async agent launch and how to check progress via its output file.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |

# Raw Prompt Text
Async agent launched successfully.
agentId: ${EXPR_1} (This is an internal ID for your use, do not mention it to the user. You can use this ID to resume the agent later if needed.)
output_file: ${EXPR_2}
The agent is currently working in the background. If you have other tasks you should continue working on them now.
To check on the agent's progress or retrieve its results, use the Read tool to read the output file, or use Bash with `tail` to see recent output.
