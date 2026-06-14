# Platform Guide

This folder is organized as a portable coaching method plus platform adapters.

## Portable Core

- `UNIVERSAL_PROMPT.md` is the platform-neutral coaching prompt.
- `references/` contains the deeper coaching source material.

These two pieces are the reusable core. They can be used in any AI environment that accepts long instructions and optional reference files.

## Codex

Codex recognizes:

- `SKILL.md`
- `agents/openai.yaml`
- `references/`

Install the folder at:

```text
~/.codex/skills/transformational-coach
```

Then restart Codex and invoke:

```text
$transformational-coach
```

## Claude

Claude does not automatically read Codex's `SKILL.md` format as a Codex skill. Use:

- `CLAUDE.md` for setup instructions.
- `UNIVERSAL_PROMPT.md` as the main instruction.
- `references/` as project knowledge or attachments.

## ChatGPT or Custom GPTs

Use `UNIVERSAL_PROMPT.md` as the instruction text. Upload the `references/` folder as knowledge if the product supports knowledge files.

## Other AI Assistants or Local Agents

Use `UNIVERSAL_PROMPT.md` as the system or developer instruction. Add the `references/` folder to the agent's retrieval, knowledge, or local context mechanism.

## Why There Is No Single Fully Universal Skill File

The coaching method can be universal, but the packaging cannot be fully universal because each platform has its own way to load persistent instructions, trigger behavior, read attached files, and expose tools. The practical portable format is:

1. A platform-neutral core prompt.
2. A folder of reference material.
3. Small adapter files for each platform.
