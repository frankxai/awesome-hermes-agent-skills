# AGENTS.md

## Repo Role

- Repo: `frankxai/awesome-hermes-agent-skills`
- Class: public companion skill-pack index for Hermes Agent
- Default health command: `git diff --check`
- Remote: `https://github.com/frankxai/awesome-hermes-agent-skills`

This repo is currently an empty companion repository. Do not describe it as a
complete skill marketplace until it contains curated skills, provenance notes,
and a validation path.

## Publishing Rules

- Each skill should live in its own folder with `SKILL.md`.
- Each skill needs purpose, inputs, outputs, required tools, safety boundaries,
  and provenance.
- Avoid copying private FrankX/Starlight runtime state, tokens, or internal
  strategy into public skill examples.
- Link back to `awesome-hermes-agents` for operator guidance and
  `NousResearch/hermes-agent` for official engine behavior.
