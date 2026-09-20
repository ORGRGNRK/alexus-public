# Who writes ALEXUS

Chris owns the repo and the machine. Three model seats write against it.

| Seat | Where the commits actually live | How they show up in git |
|---|---|---|
| Claude (Anthropic) | Private `ORGRGNRK/ALEXUS` | Author `Claude <noreply@anthropic.com>` on some commits; `Co-Authored-By: Claude … <noreply@anthropic.com>` on most of the rest |
| OpenAI (Codex / GPT) | Private `ORGRGNRK/ALEXUS` | `Co-Authored-By: Codex <noreply@openai.com>`; Codex-authored branches merged as-is; conveyor has a `codex` driver/verifier seat |
| Grok (xAI) | This public repo, and any later private commits made through the GitHub connector | Committer is `ORGRGNRK`. Message trailer `Co-Authored-By: Grok 4.6 <grok@x.ai>` |
| Chris | Both | Author `Chris` / `ORGRGNRK` `<origin@rgnrk.co>` |

GitHub will not draw Claude or OpenAI avatars on this public repo unless those CLIs commit here themselves. The private tree stays private on purpose.

Council split that the private router was built around: Claude for structure and reasoning, Grok for market/momentum, GPT/Codex for ops and for the seat that has no stake in a rule it is asked to audit.

## Claude trail already on private ALEXUS (examples, 2026)

These SHAs exist on `ORGRGNRK/ALEXUS`. They are not copied here.

- `ce8248b` — Momentum deal analyzer — author Claude
- `a5a42ea` — retail Agent 2 formulas / MPG — author Claude
- `489b6b1` — GROK First Pass Triage — author Claude
- `4076efb` — machine writers stamp Write Log Session — Co-Authored-By Claude Opus 5
- `74299b8` — conveyor Human/Machine read — Co-Authored-By Claude Opus 5
- `6f4107b` — prose-drift unmeasured runs — Co-Authored-By Claude Opus 5
- `207b2c2` — fix-drift Reminders join — Co-Authored-By Claude Opus 5
- `61b6d46` — session-walker armed — Co-Authored-By Claude Opus 5
- `920d6fe` — boot paths → Session Boot Procedure — Co-authored-by Claude

## OpenAI / Codex trail already on private ALEXUS (examples, 2026)

- `ba0c729` — airtable-mcp archive-before-canon-edit guard — Author: Codex; Co-Authored-By Codex + Claude
- `839138f` — merge `codex/thread-switch-skill` (repo-grounded handoff) — Codex authored, merged unmodified
- `9267841` — read-only Codex thread-switch skill
- `8abdf38` — conveyor `codex` driver/verifier seat (JSONL extract so echoed prompts cannot poison verdicts)
- Router GPT: Execute branch (wired to OpenAI credentials; operational, not always the git author)

Full messages stay in the private repo.

## Grok trail on this public repo

- Initial public surface (README, LICENSE, NOTICE)
- This file (Claude + OpenAI + Grok named)

Later Grok work that is safe to publish lands here with the Grok trailer.
