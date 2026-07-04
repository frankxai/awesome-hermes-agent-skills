# Awesome Hermes Agent Skills

Curated skill packs for Hermes Agent operators.

This repository is reserved for reusable `SKILL.md` packs that can be paired
with Hermes Agent profiles. It is a companion to
[`awesome-hermes-agents`](https://github.com/frankxai/awesome-hermes-agents),
which holds the broader operator guide, deployment patterns, and provenance
notes.

Official Hermes Agent behavior belongs to
[`NousResearch/hermes-agent`](https://github.com/NousResearch/hermes-agent).

## Status

Seed repository. Skills should be added only when they include:

- a clear `SKILL.md`;
- expected inputs and outputs;
- required tools or providers;
- safety and credential boundaries;
- source/provenance notes;
- a lightweight validation path.

## Planned Structure

```text
skills/
  hermes-kanban-coordinator/
    SKILL.md
  hermes-profile-doctor/
    SKILL.md
  hermes-github-pr-operator/
    SKILL.md
```

## Relationship To The Hermes Repos

| Repo | Role |
| --- | --- |
| `frankxai/hermes` | FrankX/Starlight profile specs and control-plane experiments |
| `frankxai/hermes-cockpit` | Visual registry and cockpit surface |
| `frankxai/awesome-hermes-agents` | Public operator guide and deployment patterns |
| `frankxai/awesome-hermes-agent-skills` | Reusable skill packs |

## Contribution Standard

Open a PR with one skill folder at a time. Keep examples generic and avoid
private runtime state, credentials, customer data, or internal strategy.
