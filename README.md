# lm-agent-skills

Public, agent-facing skill-pack mirror for AI Profit Machine managed agents.

**Provisioning** means pulling the latest agent-readable skill pack into a consumer agent (Grok Bot, Claude, Hermes, or a Mastra **consumer**). It is **not** a product SKU, family, domain, billing line, or checkout.

Authoring source of truth remains the private APM monorepo (`.agents/skills/managed-agents/`). This repository is the public mirror agents should fetch from. Mastra appears here only as a **consumer** mount.

## Canonical public fetch

```text
https://raw.githubusercontent.com/rapidstartup/lm-agent-skills/main/managed-agents/<pack>/SKILL.md
```

Example (Marketing Agent + Email Drafter):

```text
https://raw.githubusercontent.com/rapidstartup/lm-agent-skills/main/managed-agents/marketing-agent/SKILL.md
```

An external agent fetches that markdown and mounts it as skill/instructions.

## Layout

| Path | Role |
|---|---|
| `llms.txt` | Short catalogue of packs |
| `index.md` | Root pack index + URL pattern |
| `managed-agents/` | Managed-agent skill packs |
| `managed-agents/marketing-agent/SKILL.md` | Marketing Agent + Email Drafter provider pack |

## What this is not

- Not a GrokBot / Hermes / Mastra / OpenClaw product family
- Not a claim that APM landers are powered by Mastra (Mastra is a **consumer** mount)
- Not a change to `/managed-agents` hire or billing
- Not invented SKUs, domains, or checkout flows
