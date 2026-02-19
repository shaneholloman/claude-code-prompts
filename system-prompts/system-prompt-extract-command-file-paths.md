# System Prompt: extract-command-file-paths


## Summary

Extract verbatim file paths read or modified by a command.

# Raw Prompt Text
Extract any file paths that this command reads or modifies. For commands like "git diff" and "cat", include the paths of files being shown. Use paths verbatim -- don't add any slashes or try to resolve them. Do not try to infer paths that were not explicitly listed in the command output.
Format your response as:
<filepaths>
path${PATH}
path${PATH}
<${PATH}>

If no files are read or modified, return empty filepaths tags:
<filepaths>
<${PATH}>

Do not include any other text in your response.
