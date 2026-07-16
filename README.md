<p align="center">
  <img src="./hero.jpg" width="100%" alt="Awesome Hermes Agent Skills Hero Banner" />
</p>

<h1 align="center">✦ Awesome Hermes Agent Skills</h1>

<p align="center">
  <strong>Reusable <code>SKILL.md</code> packs, Skill Portfolio OS, and open-core free skills for <a href="https://github.com/NousResearch/hermes-agent">Hermes Agent</a> profiles.</strong>
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="https://github.com/frankxai/awesome-hermes-agent-skills/actions/workflows/link-checker.yml"><img src="https://github.com/frankxai/awesome-hermes-agent-skills/actions/workflows/link-checker.yml/badge.svg" alt="Link Check"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
  <a href="https://frankx.ai"><img src="https://img.shields.io/badge/Maintained%20by-FrankX-0ea5e9?style=flat" alt="FrankX"></a>
</p>

<p align="center">
  <a href="#-agents-vs-skills">Agents vs Skills</a> ·
  <a href="#-free-packs-in-this-repo">Free packs</a> ·
  <a href="#-skill-portfolio-os">Portfolio OS</a> ·
  <a href="#-install">Install</a> ·
  <a href="#-related-skill-ecosystem">Ecosystem</a>
</p>

---

> **Independent FrankX / Starlight curation — not official Nous Research.**  
> Official skills docs: [Skills feature](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills) · [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills)

---

## ✦ Agents vs Skills

| Repo | Role |
| --- | --- |
| **[awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents)** | **How you run agents** — profiles, Kanban, deploy, operator decision guides, swarm configs |
| **[awesome-hermes-agent-skills](https://github.com/frankxai/awesome-hermes-agent-skills)** ← *you are here* | **What agents load** — `SKILL.md` packs, free vs gated portfolio, publish playbook |

If you need installation, Windows desktop, Railway/Vercel topology, or profile armies → go to the **agents** repo.  
If you need skill packs, classification, or maintenance loops → stay here.

Community skill directories (complementary, not replacements):

- [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent)
- [SamurAIGPT/awesome-hermes-agent](https://github.com/SamurAIGPT/awesome-hermes-agent)

---

## ✦ Free packs in this repo

Install by copying a folder into your Hermes skills directory, then reload skills or start a new session.

| Pack | Description | Path |
| :--- | :--- | :--- |
| **coding-agents-superpack** | Multi-CLI discovery, structured prompts, Model Council handoffs (sanitized free) | [`skills/coding-agents-superpack`](./skills/coding-agents-superpack/SKILL.md) |
| **todo-discipline** | Hard gate: task list must match reality before “done” | [`skills/todo-discipline`](./skills/todo-discipline/SKILL.md) |

**Open-core rule:** stranger can run it with **no Frank secrets** → free. Private production / brand / personal → gated. Named buyer + support → product.

---

## ✦ Skill Portfolio OS

**GitHub SSOT:** this repo → [`docs/skill-portfolio-os/`](./docs/skill-portfolio-os/)

Read in order:

1. [STORAGE-TAXONOMY.md](./docs/skill-portfolio-os/STORAGE-TAXONOMY.md) — where durable skill docs must live  
2. [CLASSIFICATION.md](./docs/skill-portfolio-os/CLASSIFICATION.md) — free / open-core / gated / private / product  
3. [MAINTENANCE.md](./docs/skill-portfolio-os/MAINTENANCE.md) — dual-tree ops, pins, refresh  
4. [SELF-LEARNING-LOOP.md](./docs/skill-portfolio-os/SELF-LEARNING-LOOP.md) — absorb → improve → promote  
5. [PRODUCT-MAP.md](./docs/skill-portfolio-os/PRODUCT-MAP.md) — public SKU map  
6. [PUBLISH-PLAYBOOK.md](./docs/skill-portfolio-os/PUBLISH-PLAYBOOK.md) — sanitize and ship free packs  

> Do **not** treat estate control-plane paths as skill SoT. Durable public skill systems live in **this GitHub repo**.

---

## ✦ Install

Typical Hermes homes:

| OS | Skills location (default install) |
| --- | --- |
| Windows | `%LOCALAPPDATA%\hermes\skills\` (or profile-scoped skills under Hermes home) |
| macOS / Linux | `~/.hermes/skills/` or profile home skills dir |

```bash
# Example
git clone https://github.com/frankxai/awesome-hermes-agent-skills.git
cp -R awesome-hermes-agent-skills/skills/todo-discipline ~/.hermes/skills/
# reload skills / new session, then invoke by skill name
```

Authoring rules (each pack folder):

- `SKILL.md` with purpose, when-to-use, steps, tools, safety boundaries, provenance  
- No private tokens, no internal strategy dumps, no machine-local absolute secrets  
- Prefer portable process excellence over brand-locked production CoE kits  

Official reference: [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills)

---

## ✦ Related skill ecosystem

| Resource | Notes |
| --- | --- |
| [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | Runtime that loads skills |
| [agentskills.io](https://agentskills.io) | Cross-agent skill standard |
| [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) | Operator playbook companion |
| [claude-skills-library](https://github.com/frankxai/claude-skills-library) | Claude free-skills sibling |
| [agentic-creator-os](https://github.com/frankxai/agentic-creator-os) | Creator OS open core |
| [awesome-automation-agent-skills](https://github.com/frankxai/awesome-automation-agent-skills) | Loops / cron / fleet skill lists |

### FrankX awesome suite (skills-heavy)

| List | Focus |
| --- | --- |
| [awesome-hermes-agent-skills](https://github.com/frankxai/awesome-hermes-agent-skills) | **This repo** |
| [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) | Hermes agents & ops |
| [awesome-design-agent-skills](https://github.com/frankxai/awesome-design-agent-skills) | Design |
| [awesome-music-agent-skills](https://github.com/frankxai/awesome-music-agent-skills) | Music |
| [awesome-motion-design-agent-skills](https://github.com/frankxai/awesome-motion-design-agent-skills) | Motion |
| [awesome-automation-agent-skills](https://github.com/frankxai/awesome-automation-agent-skills) | Automation / loops |
| [awesome-wealth-agent-skills](https://github.com/frankxai/awesome-wealth-agent-skills) | Wealth |
| [awesome-investor-agent-skills](https://github.com/frankxai/awesome-investor-agent-skills) | Investor |
| [awesome-gamification-agent-skills](https://github.com/frankxai/awesome-gamification-agent-skills) | Gamification |
| [awesome-mind-agent-skills](https://github.com/frankxai/awesome-mind-agent-skills) | Mind |
| [awesome-manifestation-skills](https://github.com/frankxai/awesome-manifestation-skills) | Manifestation |
| [awesome-agentic-income](https://github.com/frankxai/awesome-agentic-income) | Income systems |
| [awesome-ai-coe](https://github.com/frankxai/awesome-ai-coe) | AI CoE |
| [awesome-agent-operating-systems](https://github.com/frankxai/awesome-agent-operating-systems) | Agent OS landscape |
| [awesome-cosmos-ai-agents](https://github.com/frankxai/awesome-cosmos-ai-agents) | Cosmos agents |

---

## ✦ Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) and [GETTING_STARTED.md](./GETTING_STARTED.md).

- New free packs → PR with `skills/<name>/SKILL.md` + provenance  
- Ops / deploy / profiles → [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents)  
- No secrets, no private runtime dumps, no unverified tools  

---

## ✦ License

[MIT](./LICENSE) — FrankX / Starlight

---

<p align="center">
  <sub>Built by <a href="https://github.com/frankxai">frankxai</a> · Companion ops: <a href="https://github.com/frankxai/awesome-hermes-agents">awesome-hermes-agents</a> · Runtime: <a href="https://github.com/NousResearch/hermes-agent">NousResearch/hermes-agent</a></sub>
</p>
