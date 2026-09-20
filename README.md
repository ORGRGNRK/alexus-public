# ALEXUS

Public surface for **ALEXUS** — the AI layer of RAGNAROK.

This is not the working tree.

Operational code, MCP servers, agent prompts, n8n workflows, boot skills,
intent execution, and local config live in a **private** repo and on the
machine. Yggdrasil (Airtable) is the source of truth for schema, boot, and
rules. This public repo exists so the project can be named, linked, and
starred without dumping the stack.

## What ALEXUS is

Agent infrastructure around a personal OS:

- Intent queue → approve → execute → receipt
- MCP tools against Yggdrasil
- Scoped bots (one closed loop each)
- Voice / typed route into the same executor
- Apps that grew out of that path (portal, visual continuity)

Built from zero in 2026. One machine. One owner.

## What is not here

Not published on purpose:

- MCP server source and env loading
- Airtable PATs, base IDs, bridge keys
- n8n workflow exports
- Agent system prompts and slash-command definitions
- Host paths, Tailscale addresses, port maps
- `.env`, supervisor configs, live service lists

If you need any of that, you already have access to the private tree.
If you don't, you aren't supposed to.

## Layout (private tree, for orientation only)

```
packages/    airtable-mcp, bridge, intent-executor, intent-mirror,
             bots, voice-router, iphone-agent (plan only)
apps/        portal, visual-continuity-engine
agents/      prompts + workflow exports
skills/      session lifecycle definitions
docs/        audits and plans
```

Services and ports are resolved live on the host (`pm2`, `systemctl`,
`docker ps`, `ss`). They are not pinned here so this file cannot go stale
and still look authoritative.

## License

All rights reserved. See `LICENSE`.
