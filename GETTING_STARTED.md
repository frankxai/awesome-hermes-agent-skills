# Getting Started — Hermes Agent Skills

This repo is the **skills** companion to [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents).

| Want… | Use |
| --- | --- |
| Install Hermes, profiles, Kanban, deploy | [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) + [official docs](https://hermes-agent.nousresearch.com/docs/) |
| Install / author `SKILL.md` packs | **This repo** |

## 1. Install Hermes first

Follow: [Official installation](https://hermes-agent.nousresearch.com/docs/getting-started/installation)

```bash
hermes version
hermes doctor
```

## 2. Copy a free pack

```bash
git clone https://github.com/frankxai/awesome-hermes-agent-skills.git
# Windows example:
# copy skills\todo-discipline into %LOCALAPPDATA%\hermes\skills\
# macOS/Linux:
cp -R awesome-hermes-agent-skills/skills/todo-discipline ~/.hermes/skills/
```

Reload skills in Hermes (new session or `/reload-skills` when available).

## 3. Read Skill Portfolio OS

Start at [`docs/skill-portfolio-os/README.md`](docs/skill-portfolio-os/README.md).

Key rule: **not all free, not all paid** — only portable, secret-free process packs ship publicly here.

## 4. Author a skill

Official: [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills)

Minimum structure:

```text
skills/my-skill/
  SKILL.md
```

Include: name, description, when to use, steps, required tools, safety boundaries, provenance.

## 5. Upgrade path

Premium multi-agent / brand / CoE products stay gated (see frankx.ai products / private FrankX product docs). Free packs here are the portable excellence layer.

## Related

- [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents)
- [agentskills.io](https://agentskills.io)
