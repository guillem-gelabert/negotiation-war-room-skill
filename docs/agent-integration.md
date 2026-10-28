# Agent Integration

`negotiation-war-room-skill` is a platform-independent library of skill instructions, prompts, and playbooks. It can be used by agents that read documents, accept pasted system instructions, or support custom rules.

[Back to README](../README.md)

## Core files

- [SKILL.md](../SKILL.md): full skill protocol.
- [System prompt](../prompts/system-prompt.md): standalone instructions.
- [Input template](../prompts/input-template.md): negotiation background.
- [Output template](../prompts/output-template.md): standard output.
- [Playbooks](../playbooks/): load by scenario.
- [Templates](../templates/): WeChat, email, phone, meeting, and other reusable text.

## ChatGPT

1. Paste `prompts/system-prompt.md` into a custom GPT's Instructions.
2. Upload `SKILL.md` and relevant supporting files as knowledge.
3. Use `prompts/input-template.md` for user input.

```text
Use the negotiation-war-room-skill workflow.
My negotiation background:
[complete the input template]
```

## Claude

1. Add `SKILL.md`, `prompts/`, `frameworks/`, and `playbooks/` to a Claude Project.
2. Paste the system prompt into Project Instructions.
3. Ask Claude to read the relevant playbook for each scenario.

```text
Read SKILL.md, then playbooks/client-discount.md, and help with this client discount negotiation.
```

## Cursor

1. Put the repository in the workspace.
2. Reference `SKILL.md` in Cursor Rules or project instructions.
3. Have Cursor read the relevant files for the task.

```text
Use negotiation-war-room-skill. Read SKILL.md first, then use frameworks and playbooks based on my negotiation scenario.
```

## Codex

1. Use the repository as the workspace.
2. Ask Codex to read `SKILL.md`.
3. Load relevant playbooks, frameworks, and templates.

```text
Use this repository's negotiation-war-room-skill.
Read SKILL.md, then the playbook for my scenario, and provide a full negotiation strategy.
```

## OpenAI agents

1. Use `prompts/system-prompt.md` as system instructions.
2. Put `SKILL.md`, `frameworks/`, `playbooks/`, and `templates/` in retrievable knowledge or file context.
3. Route the scenario before loading its playbook in the tool workflow.

```text
system: [prompts/system-prompt.md]
retrieval/context: SKILL.md + frameworks + playbooks + templates
user: [input-template]
assistant: [output-template]
```

## Other agents with custom instructions

Any of these capabilities can support use:

- Pasted system instructions.
- Uploaded or readable Markdown.
- Project rules.
- Local file retrieval.
- Prompt templates.

Minimal integration:

```text
System instructions: copy prompts/system-prompt.md
User input: complete prompts/input-template.md
Output format: follow prompts/output-template.md
```

## Platform-independent principles

The agent should:

1. Diagnose before drafting.
2. Identify gaps without inventing facts.
3. Analyze power, BATNA/ZOPA, and bargaining assets before offers.
4. Provide multiple offers and scores.
5. Review risks and confirm outcomes.
6. Respect safety boundaries.
