# Getting started — ninety seconds to one named skill

This is a **web-first catalog**. The value is other people's packs. Do not start at a 1,000-skill library.

Machine-readable start set: [`docs/earned.json`](./docs/earned.json)  
Always-do contract: [`docs/LIST-CONTRACT.md`](./docs/LIST-CONTRACT.md)

## 1. Hermes runs

[Official install](https://hermes-agent.nousresearch.com/docs/getting-started/installation)

```bash
hermes version
hermes doctor
```

## 2. Scanner before copy

NVIDIA's own research: **26.1%** of public skills have a vulnerability; **5.2%** look malicious. Scan first.

```bash
uv tool install git+https://github.com/NVIDIA/skillspector.git
skillspector scan https://github.com/obra/superpowers --no-llm
```

`--no-llm` is static-only (no file contents leave the machine). A clean score is a **signal**, not a warranty. `DO_NOT_INSTALL` means stop.

## 3. Install **one** named pack

Pick from [`docs/EARNED-SKILLS.md`](./docs/EARNED-SKILLS.md), not from a directory:

| Job | Pack |
| --- | --- |
| Methodology | [obra/superpowers](https://github.com/obra/superpowers) |
| Product / design / QA loops | [garrytan/gstack](https://github.com/garrytan/gstack) |
| Official named examples | [anthropics/skills](https://github.com/anthropics/skills) (one skill, not the tree) |
| Scan other skills | [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) |
| Crash-proof plans | [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) |

Follow **that repo's** README (`hermes skills install …`, `npx skills add owner/repo --skill name`, or copy one `SKILL.md` folder).

Windows skills dir is often `%LOCALAPPDATA%\hermes\skills\`. macOS/Linux: `~/.hermes/skills/`.

## 4. Directories (browse later)

[0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) · [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) · [wondelai/skills](https://github.com/wondelai/skills)

These are discovery surfaces. Do not `npx skills add` the whole tree into a business profile.

## 5. Optional packs in *this* repo

```bash
git clone https://github.com/frankxai/awesome-hermes-agent-skills.git
# copy one folder:
#   skills/todo-discipline
# into the Hermes skills directory
```

Small, secret-free, listed last. Not a replacement for the catalog.

## 6. Author your own

Official: [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills)

```text
skills/my-skill/
  SKILL.md
```

Then scan it with SkillSpector before any shared profile.
