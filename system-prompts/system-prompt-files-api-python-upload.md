# System Data Block: files-api-python-upload

- Source: native-reference-match

## Summary

System Data Block: files-api-python-upload - Source: inline Summary Upload and manage files for API requests.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `EXPR_1` | None | None |
| `EXPR_2` | None | None |
| `EXPR_3` | None | None |
| `EXPR_4` | None | None |
| `OPUS_ID` | None | None |
| `EXPR_5` | None | None |
| `EXPR_6` | None | None |
| `EXPR_7` | None | None |
| `EXPR_8` | None | None |
| `EXPR_9` | None | None |
| `EXPR_10` | None | None |
| `EXPR_11` | None | None |
| `EXPR_12` | None | None |
| `EXPR_13` | None | None |
| `EXPR_14` | None | None |
| `EXPR_15` | None | None |
| `EXPR_16` | None | None |

# Raw Prompt Text
# System Data Block: files-api-python-upload

- Source: inline

## Summary

Upload and manage files for API requests.

## Placeholder Hints (source-backed)

| Expression | Hint | Reference |
| --- | --- | --- |
| `OPUS_ID` | None | None |

# Raw Prompt Text
# Files API — Python

The Files API uploads files for use in Messages API requests. Reference files via `file_id` in content blocks, avoiding re-uploads across multiple API calls.

**Beta:** Pass `betas=["files-api-${EXPR_1}"]` in your API calls (the SDK sets the required header automatically).

## Key Facts

- Maximum file size: ${EXPR_2} MB
- Total storage: ${EXPR_3} GB per organization
- Files persist until deleted
- File operations (upload, list, delete) are free; content used in messages is billed as input tokens
- Not available on Amazon Bedrock or Google Vertex AI

---

## Upload a File

```python
import anthropic

client = anthropic.Anthropic()

uploaded = client.beta.files.upload(
    file=("report.pdf", open("report.pdf", "rb"), "application${EXPR_4}"),
)
print(f"File ID: {uploaded.id}")
print(f"Size: {uploaded.size_bytes} bytes")
```

---

## Use a File in Messages

### PDF / Text Document

```python
response = client.beta.messages.create(
    model="{{OPUS_ID}}",
    max_tokens=${EXPR_5},
    messages=[{
        "role": "user",
        "content": [
            {"type": "text", "text": "Summarize the key findings in this report."},
            {
                "type": "document",
                "source": {"type": "file", "file_id": uploaded.id},
                "title": "Q4 Report",           # optional
                "citations": {"enabled": True}   # optional, enables citations
            }
        ]
    }],
    betas=["files-api-${EXPR_6}"],
)
for block in response.content:
    if block.type == "text":
        print(block.text)
```

### Image

```python
image_file = client.beta.files.upload(
    file=("photo.png", open("photo.png", "rb"), "image${EXPR_7}"),
)

response = client.beta.messages.create(
    model="{{OPUS_ID}}",
    max_tokens=${EXPR_8},
    messages=[{
        "role": "user",
        "content": [
            {"type": "text", "text": "What's in this image?"},
            {
                "type": "image",
                "source": {"type": "file", "file_id": image_file.id}
            }
        ]
    }],
    betas=["files-api-${EXPR_9}"],
)
```

---

## Manage Files

### List Files

```python
files = client.beta.files.list()
for f in files.data:
    print(f"{f.id}: {f.filename} ({f.size_bytes} bytes)")
```

### Get File Metadata

```python
file_info = client.beta.files.retrieve_metadata("file_011CNha8iCJcU1wXNR6q4V8w")
print(f"Filename: {file_info.filename}")
print(f"MIME type: {file_info.mime_type}")
```

### Delete a File

```python
client.beta.files.delete("file_011CNha8iCJcU1wXNR6q4V8w")
```

### Download a File

Only files created by the code execution tool or skills can be downloaded (not user-uploaded files).

```python
file_content = client.beta.files.download("file_011CNha8iCJcU1wXNR6q4V8w")
file_content.write_to_file("output.txt")
```

---

## Full End-to-End Example

Upload a document once, ask multiple questions about it:

```python
import anthropic

client = anthropic.Anthropic()

# ${EXPR_10}. Upload once
uploaded = client.beta.files.upload(
    file=("contract.pdf", open("contract.pdf", "rb"), "application${EXPR_11}"),
)
print(f"Uploaded: {uploaded.id}")

# ${EXPR_12}. Ask multiple questions using the same file_id
questions = [
    "What are the key terms and conditions?",
    "What is the termination clause?",
    "Summarize the payment schedule.",
]

for question in questions:
    response = client.beta.messages.create(
        model="{{OPUS_ID}}",
        max_tokens=${EXPR_13},
        messages=[{
            "role": "user",
            "content": [
                {"type": "text", "text": question},
                {
                    "type": "document",
                    "source": {"type": "file", "file_id": uploaded.id}
                }
            ]
        }],
        betas=["files-api-${EXPR_14}"],
    )
    print(f"\nQ: {question}")
    text = next((b.text for b in response.content if b.type == "text"), "")
    print(f"A: {text[:${EXPR_15}]}")

# ${EXPR_16}. Clean up when done
client.beta.files.delete(uploaded.id)
```
