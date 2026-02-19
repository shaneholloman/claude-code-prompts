# System Prompt: batch-invocations-guide

- Source: inline

## Summary

Defines parallel batch tool invocations list, aggregating results and requiring post-call user message.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | Bash | None |
| `EXPR_3` | GlobTool | None |
| `EXPR_4` | GrepTool | None |

# Raw Prompt Text
- Batch execution tool that runs multiple tool invocations in a single request
- Tools are executed in parallel when possible, and otherwise serially
- Takes a list of tool invocations (tool_name and input pairs)
- Returns the collected results from all invocations
- Use this tool when you need to run multiple independent tool operations at once -- it is awesome for speeding up your workflow, reducing both context usage and latency
- Each tool will respect its own permissions and validation rules
- The tool's outputs are NOT shown to the user; to answer the user's query, you MUST send a message with the results after the tool call completes, otherwise the user will not see the results

Available tools:
${EXPR_1}

Example usage:
{
  "invocations": [
    {
      "tool_name": "${EXPR_2: 'Bash'}",
      "input": {
        "command": "git blame src${PATH}"
      }
    },
    {
      "tool_name": "${EXPR_3: 'GlobTool'}",
      "input": {
        "pattern": "**/*.ts"
      }
    },
    {
      "tool_name": "${EXPR_4: 'GrepTool'}",
      "input": {
        "pattern": "function",
        "include": "*.ts"
      }
    }
  ]
}
