# AGENTS.md

## Repo Role

- Repo: `frankxai/awesome-hermes-agent-skills`
- Class: public companion **skill-pack** index + Skill Portfolio OS for Hermes Agent
- Remote: `https://github.com/frankxai/awesome-hermes-agent-skills`
- Companion ops list: `https://github.com/frankxai/awesome-hermes-agents`

## Split

| Concern | Repo |
| --- | --- |
| Profiles, Kanban, deploy, operator guides | awesome-hermes-agents |
| SKILL.md packs, portfolio OS, free vs gated | **this repo** |

## Publishing Rules

- Each skill lives in `skills/<name>/SKILL.md` (plus optional references/scripts).
- Each skill needs purpose, inputs, outputs, required tools, safety boundaries, and provenance.
- Avoid copying private FrankX/Starlight runtime state, tokens, or internal strategy into public skill examples.
- Link back to `awesome-hermes-agents` for operator guidance and `NousResearch/hermes-agent` for official engine behavior.
- Skill Portfolio OS SSOT: `docs/skill-portfolio-os/` (not estate `starlight/ops` redirects).

## Default health

- `git diff --check`
- Prefer draft PRs for large README churn; batch docs commits with `[skip ci]` only when CI is pure link-check noise and links were verified locally.
