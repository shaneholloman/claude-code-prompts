# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Tool Description: lsp-intelligence-operations-… - Source: native-reference-match Summary Use LSP to navigate symbols, references, hover, and call hierarchy i…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Tool Description: lsp

- Source: native-reference-match

## Summary

Use LSP to navigate symbols, references, hover, and call hierarchy in code.

# Raw Prompt Text
Interact with Language Server Protocol (LSP) servers to get code intelligence features.

Supported operations:
- goToDefinition: Find where a symbol is defined
- findReferences: Find all references to a symbol
- hover: Get hover information (documentation, type info) for a symbol
- documentSymbol: Get all symbols (functions, classes, variables) in a document
- workspaceSymbol: Search for symbols across the entire workspace
- goToImplementation: Find implementations of an interface or abstract method
- prepareCallHierarchy: Get call hierarchy item at a position (functions${EXPR_1})
- incomingCalls: Find all functions${EXPR_2} that call the function at a position
- outgoingCalls: Find all functions${EXPR_3} called by the function at a position

All operations require:
- filePath: The file to operate on
- line: The line number (${EXPR_4}-based, as shown in editors)
- character: The character offset (${EXPR_5}-based, as shown in editors)

Note: LSP servers must be configured for the file type. If no server is available, an error will be returned.
