# Tool Description: language-server-intelligence

- Name: LSP

## Summary

Provides LSP-based navigation and symbol queries using file position inputs.

# Raw Prompt Text
Interact with Language Server Protocol (LSP) servers to get code intelligence features.

Supported operations:
- goToDefinition: Find where a symbol is defined
- findReferences: Find all references to a symbol
- hover: Get hover information (documentation, type info) for a symbol
- documentSymbol: Get all symbols (functions, classes, variables) in a document
- workspaceSymbol: Search for symbols across the entire workspace

All operations require:
- filePath: The file to operate on
- line: The line number (${NUM}-indexed)
- character: The character offset (${NUM}-indexed) on the line

Note: LSP servers must be configured for the file type. If no server is available, an error will be returned.
