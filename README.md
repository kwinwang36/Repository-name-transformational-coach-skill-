# Transformational Coach Skill

A portable transformational coaching method with a Codex skill adapter.

This skill helps an AI assistant act as a coach rather than an advice-giver. It guides users through rapport, contract setting, outcome clarification, values exploration, logical levels, commitment, action design, and completion.

The folder now has two layers:

- `UNIVERSAL_PROMPT.md`: the platform-neutral core prompt. Use this in Claude, ChatGPT, Gemini, local agents, or any assistant that accepts custom instructions.
- `SKILL.md`: the Codex adapter, so the same method still works as a local Codex skill.

## What It Helps With

- Clarifying priorities when daily tasks feel chaotic
- Exploring interests, values, and life direction
- Sustaining long-term goals when urgent tasks interrupt progress
- Starting a new skill-learning plan
- Making career or life choices
- Turning complaints into desired outcomes and controllable next steps

## Universal Use

Use `UNIVERSAL_PROMPT.md` as the main instruction in any AI tool. If the tool supports project knowledge, files, or retrieval, also add the `references/` folder.

For Claude, see `CLAUDE.md`.

For platform-specific setup details, see `PLATFORM_GUIDE.md`.

## Codex Install

Download this repository and place the folder in your Codex skills directory.

Windows:

```text
C:\Users\<your-name>\.codex\skills\transformational-coach
```

macOS / Linux:

```text
~/.codex/skills/transformational-coach
```

The final folder structure should look like this:

```text
transformational-coach/
  SKILL.md
  agents/
    openai.yaml
  references/
    00-source-reading-notes.md
    01-principles-and-stance.md
    ...
```

Restart Codex or start a new conversation after installing.

## Codex Usage

Invoke the skill explicitly:

```text
$transformational-coach 我现在被很多琐事推着走，不知道今天到底该优先处理什么，请你用教练方式带我澄清。
```

Other examples:

```text
$transformational-coach 我想探索自己真正热爱的方向，但现在脑子很乱，请你带我完成一次教练对话。
```

```text
$transformational-coach 我有一个三个月瘦身目标，但总是被事情打断，帮我通过教练对话找到可坚持的行动承诺。
```

## Notes

There is no single skill file that every AI platform automatically recognizes. The portable part is the coaching prompt and reference material; each platform needs a small adapter or setup step.

The complete source reading notes are preserved in `references/00-source-reading-notes.md` for deeper use and future extension.
