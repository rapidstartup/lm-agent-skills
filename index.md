# lm-agent-skills — pack index

Provisioning = skill-pack pull from this public mirror. It is not a SKU, family, domain, or checkout.

Authoring SoT: private APM monorepo `.agents/skills/managed-agents/`. This repo is the agent-facing public mirror. Mastra = consumer only.

## Canonical public URL pattern

```text
https://raw.githubusercontent.com/rapidstartup/lm-agent-skills/main/managed-agents/<pack>/SKILL.md
```

Replace `<pack>` with a directory name from the table below.

## Packs

| Pack | Use when | Public URL |
|---|---|---|
| `marketing-agent` | Mounting APM Marketing Agent and/or Email Drafter as draft-only capabilities on Claude, Grok Bot, Hermes, or a Mastra consumer | https://raw.githubusercontent.com/rapidstartup/lm-agent-skills/main/managed-agents/marketing-agent/SKILL.md |

See [README.md](./README.md) and [managed-agents/README.md](./managed-agents/README.md).
