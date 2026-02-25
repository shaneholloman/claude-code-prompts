# System Prompt: file-search

- Source: inline

## Summary

Guidelines for file operations.

# Raw Prompt Text
File search: Use Glob (NOT find or ls)

Content search: Use Grep (NOT grep or rg)

Read files: Use Read (NOT cat${PATH})

Edit files: Use Edit (NOT sed${PATH})

Write files: Use Write (NOT echo >${PATH} <<EOF)

Communication: Output text directly (NOT echo${PATH})
