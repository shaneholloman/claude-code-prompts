# System Data Block: files-api-typescript-overview

- Source: native-reference-match

## Summary

System Data Block: files-api-typescript-overview - Source: native-reference-match Summary System Data Block: files-api-typescript-upload - Source: inline Sum…

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `OPUS_ID` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
# System Data Block: files-api-typescript-overview

- Source: native-reference-match

## Summary

System Data Block: files-api-typescript-upload - Source: inline Summary Overview of the Files API for file uploads.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `OPUS_ID` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |
| `EXPR_17` | None | None |

# Raw Prompt Text
# System Data Block: files-api-typescript-upload

- Source: inline

## Summary

Overview of the Files API for file uploads.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `OPUS_ID` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `EXPR_5` | None | None |

# Raw Prompt Text
# Files API — TypeScript

The Files API uploads files for use in Messages API requests. Reference files via `file_id` in content blocks, avoiding re-uploads across multiple API calls.

**Beta:** Pass `betas: ["files-api-${EXPR_1}"]` in your API calls (the SDK sets the required header automatically).

## Key Facts

- Maximum file size: ${EXPR_2} MB
- Total storage: ${EXPR_3} GB per organization
- Files persist until deleted
- File operations (upload, list, delete) are free; content used in messages is billed as input tokens
- Not available on Amazon Bedrock or Google Vertex AI

---

## Upload a File

```typescript
import Anthropic, { toFile } from "@anthropic-ai${EXPR_4}";
import fs from "fs";

const client = new Anthropic();

const uploaded = await client.beta.files.upload({
  file: await toFile(fs.createReadStream("report.pdf"), undefined, {
    type: "application${EXPR_5}",
  }),
  betas: ["files-api-${EXPR_6}"],
});

console.log(`File ID: ${EXPR_7}`);
console.log(`Size: ${EXPR_8} bytes`);
```

---

## Use a File in Messages

### PDF / Text Document

```typescript
const response = await client.beta.messages.create({
  model: "{{OPUS_ID}}",
  max_tokens: ${EXPR_9},
  messages: [
    {
      role: "user",
      content: [
        { type: "text", text: "Summarize the key findings in this report." },
        {
          type: "document",
          source: { type: "file", file_id: uploaded.id },
          title: "Q4 Report",
          citations: { enabled: true },
        },
      ],
    },
  ],
  betas: ["files-api-${EXPR_10}"],
});

console.log(response.content[${EXPR_11}].text);
```

---

## Manage Files

### List Files

```typescript
const files = await client.beta.files.list({
  betas: ["files-api-${EXPR_12}"],
});
for (const f of files.data) {
  console.log(`${EXPR_13}: ${EXPR_14} (${EXPR_15} bytes)`);
}
```

### Delete a File

```typescript
await client.beta.files.delete("file_011CNha8iCJcU1wXNR6q4V8w", {
  betas: ["files-api-${EXPR_16}"],
});
```

### Download a File

```typescript
const response = await client.beta.files.download(
  "file_011CNha8iCJcU1wXNR6q4V8w",
  { betas: ["files-api-${EXPR_17}"] },
);
const content = Buffer.from(await response.arrayBuffer());
await fs.promises.writeFile("output.txt", content);
```
