# ALEXUS

Public surface for **ALEXUS** — the AI layer of RAGNAROK.

This is not the working tree.

Operational code, MCP servers, agent prompts, n8n workflows, boot skills,
intent execution, and local config live in a **private** repo and on the
machine. Yggdrasil (Airtable) is the source of truth for schema, boot, and
rules. This public repo exists so the project can be named, linked, and
starred without dumping the stack.

## About

**ALEXUS**, built by Chris (ORGRGNRK) in 2026, uses Claude, OpenAI, and Grok for code. **Yggdrasil** is the source of truth. This public surface omits private stack details. Licensed under **MIT**.

## Seats

Built by Chris with Claude, OpenAI (Codex / GPT), and Grok. All three model seats write code. See `CONTRIBUTORS.md`.

- **Claude** — structure, reasoning, most of the private tree. Real git author on several private commits (`Claude <noreply@anthropic.com>`), Co-Authored-By on the rest.
- **OpenAI (Codex / GPT)** — ops, auditor seat with no stake in the rule it is asked to bind, conveyor `codex` seat, thread-switch skill. Trailer `Co-Authored-By: Codex <noreply@openai.com>`.
- **Grok** — market/momentum lane, and this public surface through the GitHub connector. Committer is the owner account. Trailer: `Co-Authored-By: Grok 4.6 <grok@x.ai>`.
- **Chris** — builder, creator, and owner of ALEXUS. Decides what gets built, works through problems with the model seats, and owns every merge and every machine.

Do not expect Claude or OpenAI GitHub users to appear in the contributor graph here. Those identities are on the private repo. Copying that history public would publish the stack.

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

## License

MIT License. See `LICENSE`.
