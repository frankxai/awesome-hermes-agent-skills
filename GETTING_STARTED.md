# Getting Started — Hermes Agent Skills

This is a **web-first skills catalog**. Most of the value is links to other people's skill packs.

| Want… | Use |
| --- | --- |
| Start with 5–7 earned skills | [docs/EARNED-SKILLS.md](./docs/EARNED-SKILLS.md) |
| Safety before install | [docs/QUALITY-AND-SAFETY.md](./docs/QUALITY-AND-SAFETY.md) + [NVIDIA SkillSpector](https://github.com/NVIDIA/SkillSpector) |
| Browse the web-first catalog | [README.md](./README.md) sections above “Maintained in this repo” |
| Broader directories (do not bulk-install) | [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) · [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) |
| Agents / UIs / deploy | [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) |
| Official skill authoring | [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills) |

## 1. Install Hermes

[Official installation](https://hermes-agent.nousresearch.com/docs/getting-started/installation)

```bash
hermes version
hermes doctor
```

## 2. Install a skill from the web (preferred path)

Pick **one named skill**, not a 1,000-skill catalog. Start from [docs/EARNED-SKILLS.md](./docs/EARNED-SKILLS.md), e.g.:

- [anthropics/skills](https://github.com/anthropics/skills) — install a **named** official skill
- [obra/superpowers](https://github.com/obra/superpowers)
- [garrytan/gstack](https://github.com/garrytan/gstack)
- [wondelai/skills](https://github.com/wondelai/skills) if you need a Hermes-native library

Read the `SKILL.md` and scan with SkillSpector before it touches a business profile.

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
