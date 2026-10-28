# Quick Start

For first-time users: clone the repository, read the protocol, copy the system prompt, complete the input template, and check output with a test prompt in about five minutes.

[Back to README](../README.md)

## 1. Clone

```bash
git clone https://github.com/guillem-gelabert/negotiation-war-room-skill.git
cd negotiation-war-room-skill
```

You can also read the files directly on GitHub without a local installation.

## 2. Open `SKILL.md`

The core protocol defines the agent's role, workflow, input and output, safety boundaries, and usage.

```bash
cat SKILL.md
```

Read:

- [SKILL.md](../SKILL.md)
- [System prompt](../prompts/system-prompt.md)
- [Input template](../prompts/input-template.md)
- [Output template](../prompts/output-template.md)

## 3. Copy the system prompt

For tools with System Prompt, Project Instructions, Rules, or custom agent instructions, copy [prompts/system-prompt.md](../prompts/system-prompt.md).

```text
Use negotiation-war-room-skill with these instructions:
[paste prompts/system-prompt.md]
```

Otherwise, begin the conversation with:

```text
Read and follow the workflow in negotiation-war-room-skill's SKILL.md.
My background:
[paste background]
```

## 4. Complete the input template

Open [prompts/input-template.md](../prompts/input-template.md).

```text
[Type]
Client discount

[Background]
The client cites a competitor 40% cheaper and wants a discount.

[My role]
Provider's team lead with authority for up to 10% off.

[Other party]
Marketing lead, possibly needing owner approval.

[Objective]
Protect the quote; no more than 10% off.

[Limit]
A greater discount requires reduced scope.

[BATNA]
Give the team's slot to a more profitable client.

[Channel]
WeChat

[Output]
Strategy / three offers / WeChat wording / risk review
```

## 5. Try test prompts

Copy a prompt from [tests/test-prompts.md](../tests/test-prompts.md). Start with:

```text
Use negotiation-war-room-skill. The client wants 25% off or will find someone else. I can concede at most 8% but want to retain the work. Provide strategy, three offers, and a WeChat reply.
```

```text
Use negotiation-war-room-skill. A client owes RMB 100,000, delays acceptance, and raises no specific issues. I want goodwill but cannot revise for free indefinitely. Provide strategy and follow-up wording.
```

```text
Use negotiation-war-room-skill. My offer is below expectations and I want 15% more. Draft an email and review risks.
```

## 6. Assess the output

Look for scenario identification, gaps, power scoring, three-level goals, BATNA/ZOPA, bargaining map, three offers, scores, first wording, reactions and replies, pre-send review, confirmation, and next actions.

See the [acceptance checklist](../tests/acceptance-checklist.md) for full criteria.
