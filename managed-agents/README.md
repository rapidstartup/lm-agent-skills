# Managed-agent skill packs (public mirror)

**Provisioning** here means pulling the latest agent-readable skill pack from this tree into a consumer agent (Grok Bot, Claude, Hermes, or a Mastra **consumer**). It is **not** a product SKU, family, domain, billing line, or checkout.

This directory is the **agent-facing public mirror** of the authoring source of truth in the private APM monorepo (`.agents/skills/managed-agents/`). Edit packs in APM first; sync here for public fetch. Mastra is a **consumer** only.

## Canonical agent fetch

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
| `index.md` | Pack list + URL pattern |
| `marketing-agent/SKILL.md` | Marketing Agent + Email Drafter provider pack |

Grounding for the Marketing Agent pack is the draft-only runtime in APM `managed-agent-runtime/src/marketing-agent.ts` and `managed-agent-runtime/src/email-agent.ts`. That runtime has no live connectors.

## What this is not

- Not a GrokBot / Hermes / Mastra / OpenClaw product family
- Not a claim that APM landers are powered by Mastra (Mastra is a **consumer** mount)
- Not a change to `/managed-agents` hire or billing
- Not invented SKUs, domains, or checkout flows
