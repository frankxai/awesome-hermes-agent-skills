# Getting Started — Hermes Agent Skills

This is a **web-first skills catalog**. Most of the value is links to other people's skill packs.

| Want… | Use |
| --- | --- |
| Browse best skills on the web | [README.md](./README.md) sections above “Maintained in this repo” |
| Broader directories | [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) · [SamurAIGPT/awesome-hermes-agent](https://github.com/SamurAIGPT/awesome-hermes-agent) |
| Agents / UIs / deploy | [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) |
| Official skill authoring | [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills) |

## 1. Install Hermes

[Official installation](https://hermes-agent.nousresearch.com/docs/getting-started/installation)

```bash
hermes version
hermes doctor
```

## 2. Install a skill from the web (preferred path)

Pick something high-signal from the README, e.g.:

- [wondelai/skills](https://github.com/wondelai/skills)
- [Romanescu11/hermes-skill-factory](https://github.com/Romanescu11/hermes-skill-factory)
- [tlehman/litprog-skill](https://github.com/tlehman/litprog-skill)

Follow **that repo's** install instructions. Patterns you will see:

```bash
# clone + copy SKILL.md tree into Hermes skills dir
# or: hermes skills install owner/repo/...
# or: npx skills add owner/repo -g
```

## 3. Optional: free packs in *this* repo

```bash
git clone https://github.com/frankxai/awesome-hermes-agent-skills.git
cp -R awesome-hermes-agent-skills/skills/todo-discipline ~/.hermes/skills/
```

These are small open-core packs — not a replacement for the ecosystem catalog.

## 4. Author your own

Official: [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills)

Minimum:

```text
skills/my-skill/
  SKILL.md
```

## 5. Portfolio ops (maintainers)

[`docs/skill-portfolio-os/`](docs/skill-portfolio-os/) — free vs gated vs product classification for packs we publish.
