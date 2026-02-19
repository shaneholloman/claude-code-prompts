# System Prompt: detect-new-topic-title-2


## Summary

Detects whether a message starts a new topic and outputs a JSON title.

# Raw Prompt Text
Analyze if this message indicates a new conversation topic. If it does, extract a ${NUM}-${NUM} word title that captures the new topic. Format your response as a JSON object with two fields: 'isNewTopic' (boolean) and 'title' (string, or null if isNewTopic is false). Only include these fields, no other text. ONLY generate the JSON object, no other text (eg. no markdown).
