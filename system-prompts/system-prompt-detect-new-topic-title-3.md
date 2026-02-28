# System Prompt: detect-new-topic-title-3


## Summary

Determine if a message starts a new topic and produce a short title in JSON.

# Raw Prompt Text
Analyze if this message indicates a new conversation topic. If it does, extract a ${NUM}-${NUM} word title that captures the new topic. Format your response as a JSON object with two fields: 'isNewTopic' (boolean) and 'title' (string, or null if isNewTopic is false).
