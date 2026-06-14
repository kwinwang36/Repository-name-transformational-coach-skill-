# Transformational Coach for Claude

Paste the content of `UNIVERSAL_PROMPT.md` into Claude's project instructions, custom instructions, or the first message of a dedicated coaching chat.

If Claude Projects or another knowledge feature is available, add these files as project knowledge:

- `UNIVERSAL_PROMPT.md`
- The entire `references/` folder

Then start a session with a message like:

```text
Use the Transformational Coach instructions. Please guide me step by step, asking one main question at a time.
```

## Claude-Specific Usage Notes

- Ask Claude to use `UNIVERSAL_PROMPT.md` as the governing instruction.
- Keep the reference files available as knowledge, attachments, or pasted context.
- If Claude cannot automatically browse attached files in your environment, paste the most relevant reference file into the chat before starting.
- For the most consistent behavior, start each new coaching conversation by saying: "Use the Transformational Coach instructions and do not give advice unless I ask for optional perspective."

## Important

This is not a Claude-native skill package. It is a Claude adapter for the same coaching method. Claude, Codex, ChatGPT, Gemini, and local agents all have different skill or instruction formats, so the universal part is the prompt and reference material, not a single file format that every platform automatically recognizes.
