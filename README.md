<p align="center">
  <img src="./hero.jpg" width="100%" alt="Awesome Hermes Agent Skills" />
</p>

<h1 align="center">Awesome Hermes Agent Skills</h1>

<p align="center">
  <strong>A curated list of the best Hermes-compatible skills, plugins, and skill factories from across the web — plus a few free open-core packs we maintain.</strong>
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="https://github.com/frankxai/awesome-hermes-agent-skills/actions/workflows/link-checker.yml"><img src="https://github.com/frankxai/awesome-hermes-agent-skills/actions/workflows/link-checker.yml/badge.svg" alt="Link Check"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
</p>

---

> Independent curation. **Not** official Nous Research.  
> Official skill docs: [Skills](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills) · [Creating skills](https://hermes-agent.nousresearch.com/docs/developer-guide/creating-skills) · [agentskills.io](https://agentskills.io)

**This is an awesome list of the web**, not a marketing page for our packs.  
FrankX free packs are listed last under [Maintained in this repo](#maintained-in-this-repo-optional).

| Companion | Role |
| --- | --- |
| [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) | Agents, UIs, memory, deploy, multi-agent, operator docs |
| **This repo** | Skills / plugins / skill factories (web-wide) |

**Start here:** pick about five named skills. Do not install a 1,000-skill catalog.

| Pack | Job | Pulse 2026-08-30 |
| --- | --- | --- |
| [agentskills/agentskills](https://github.com/agentskills/agentskills) | Portable `SKILL.md` spec | Apache-2.0 · `reviewed` |
| [anthropics/skills](https://github.com/anthropics/skills) | Official examples — install **named** skills | `reviewed` |
| [obra/superpowers](https://github.com/obra/superpowers) | TDD, debug, review, shipping | MIT · `reviewed` |
| [garrytan/gstack](https://github.com/garrytan/gstack) | Product, design, eng, QA, browser | MIT · `reviewed` |
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Scan a skill before it runs | Apache-2.0 · `reviewed` |

Full table and domain map: [`docs/EARNED-SKILLS.md`](./docs/EARNED-SKILLS.md) · safety: [`docs/QUALITY-AND-SAFETY.md`](./docs/QUALITY-AND-SAFETY.md)

Directories (browse, do not bulk-install): [0xNyk](https://github.com/0xNyk/awesome-hermes-agent) · [SamurAIGPT](https://github.com/SamurAIGPT/awesome-hermes-agent) · [VoltAgent](https://github.com/VoltAgent/awesome-agent-skills) · [ZeroPointRepo](https://github.com/ZeroPointRepo/awesome-hermes-skills)

Maturity labels: **production** · **beta** · **experimental**  
Review states: `reviewed` · `watch` · `unverified` · `unsafe`  
Research pulse: **2026-08-30**

---

## Contents

- [Earned skills (start here)](#earned-skills-start-here)
- [Safety gate](#safety-gate)
- [How to install a skill](#how-to-install-a-skill)
- [Find skills by domain](#find-skills-by-domain)
- [Skill libraries & standards](#skill-libraries--standards)
- [Hermes-native skills & plugins](#hermes-native-skills--plugins)
- [agentskills.io & cross-harness packs](#agentskillsio--cross-harness-packs)
- [Visual production skills](#visual-production-skills)
- [Domain skill packs](#domain-skill-packs)
- [Skill factories & evolution](#skill-factories--evolution)
- [Related tools (skills-adjacent)](#related-tools-skills-adjacent)
- [August 2026 research additions](#august-2026-research-additions)
- [Directories, not installs](#directories-not-installs)
- [6-Pillar curation lens](#6-pillar-curation-lens)
- [Explore the Full FrankX Awesome Ecosystem (17 lists) (optional)](#explore-the-full-frankx-awesome-ecosystem-17-lists-optional)
- [Maintained in this repo (optional)](#maintained-in-this-repo-optional)
- [Skill Portfolio OS](#skill-portfolio-os)
- [Contributing](#contributing)

---

## Earned skills (expanded)

The compact table is at the top of this README. Full rationale: [`docs/EARNED-SKILLS.md`](./docs/EARNED-SKILLS.md).

| Pack | Job | Pulse 2026-08-30 |
| --- | --- | --- |
| [agentskills/agentskills](https://github.com/agentskills/agentskills) | Portable `SKILL.md` spec | Apache-2.0 · ~24.9k★ · `reviewed` |
| [anthropics/skills](https://github.com/anthropics/skills) | Official examples — install **named** skills | inspect license · ~173k★ · `reviewed` |
| [obra/superpowers](https://github.com/obra/superpowers) | TDD, debug, review, shipping methodology | MIT · ~280k★ · `reviewed` |
| [garrytan/gstack](https://github.com/garrytan/gstack) | Product, design, eng, QA, browser loops | MIT · ~130k★ · `reviewed` |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Production engineering skills | MIT · ~91k★ · `reviewed` |
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Scan a skill before it can run | Apache-2.0 · ~15k★ · `reviewed` |
| [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | Plans that survive compaction | MIT · ~26k★ · `reviewed` |

FrankX free packs (`todo-discipline`, `coding-agents-superpack`) are listed **last**.

## Safety gate

Skills are becoming package managers for **behavior**. Read [QUALITY-AND-SAFETY.md](./docs/QUALITY-AND-SAFETY.md) before copying anything into a live profile.

1. Open the primary repo. Confirm a real `SKILL.md` and a license.
2. Read the skill for hidden fetch/write/env/approval-bypass instructions.
3. Scan with [NVIDIA SkillSpector](https://github.com/NVIDIA/SkillSpector).
4. Install into a throwaway profile first.
5. Human-gate money, deploys, credentials, and public posts.

**Quarantine:** OpenClaw/ClawHub dumps, unsigned ZIP/S3 skill blobs, wallet/broadcast-tx packs without a dry-run + spend cap, and “install our 300–2,000 skills” operating systems.

## How to install a skill

1. Install Hermes: [official installation](https://hermes-agent.nousresearch.com/docs/getting-started/installation)  
2. Clone or copy **one** skill folder containing `SKILL.md` into your Hermes skills directory  
   - Windows: often `%LOCALAPPDATA%\hermes\skills\`  
   - macOS/Linux: often `~/.hermes/skills/`  
   - Profile-scoped skills may live under the profile home  
3. New session / reload skills; invoke by skill name  

Prefer the project's own README for exact install (`hermes skills install …`, `npx skills add …`, etc.). Do not `npx skills add` an entire 1,000-skill catalog into a production profile.

## Find skills by domain

| Need | Go here |
| --- | --- |
| Coding agents / runtimes / MCP | [awesome-agent-operating-systems](https://github.com/frankxai/awesome-agent-operating-systems) |
| Design / anti-slop UI | [awesome-design-agent-skills](https://github.com/frankxai/awesome-design-agent-skills) · [bergside/awesome-design-skills](https://github.com/bergside/awesome-design-skills) |
| Motion / Remotion / video | [awesome-motion-design-agent-skills](https://github.com/frankxai/awesome-motion-design-agent-skills) · [remotion-dev/skills](https://github.com/remotion-dev/skills) |
| Game engines | [gamedev-skills/awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) (router + **one** engine) |
| Music | [awesome-music-agent-skills](https://github.com/frankxai/awesome-music-agent-skills) |
| Payments (mandate before settle) | [awesome-payment-agent-skills](https://github.com/frankxai/awesome-payment-agent-skills) |
| Wealth / investor **research** (not advice) | [awesome-wealth-agent-skills](https://github.com/frankxai/awesome-wealth-agent-skills) · [awesome-investor-agent-skills](https://github.com/frankxai/awesome-investor-agent-skills) |
| Automation / MCP | [awesome-automation-agent-skills](https://github.com/frankxai/awesome-automation-agent-skills) |
| Science | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| GitHub Copilot | [github/awesome-copilot](https://github.com/github/awesome-copilot) |

---

## Skill libraries & standards

| Project | Maturity | Why |
| --- | --- | --- |
| [agentskills.io](https://agentskills.io) | production | Open skill standard used by Hermes + many harnesses |
| [wondelai/skills](https://github.com/wondelai/skills) | production | Large multi-harness skills library (~1.6k★) — great first install |
| [0xNyk/awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) | production | Independent directory of skills/plugins/tools |
| [SamurAIGPT/awesome-hermes-agent](https://github.com/SamurAIGPT/awesome-hermes-agent) | production | Hand-picked list with maturity tags |
| [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) skills docs | production | Built-in skill system + curator loop |

---

## Hermes-native skills & plugins

| Project | Maturity | Why |
| --- | --- | --- |
| [42-evey/hermes-plugins](https://github.com/42-evey/hermes-plugins) | beta | Goals, inter-agent bridge, model selection, cost control |
| [CorsenAI/hermes-connector](https://github.com/CorsenAI/hermes-connector) | beta | Chrome extension and local companion for exact Hermes sessions and user-selected tabs |
| [Romanescu11/hermes-skill-factory](https://github.com/Romanescu11/hermes-skill-factory) | beta | Auto-generate skills from real workflows |
| [tlehman/litprog-skill](https://github.com/tlehman/litprog-skill) | beta | Literate programming for Hermes / Claude Code / OpenCode |
| [Cranot/super-hermes](https://github.com/Cranot/super-hermes) | experimental | Teach Hermes to write stronger analytical prompts first |
| [witt3rd/oh-my-hermes](https://github.com/witt3rd/oh-my-hermes) | beta | Orchestration skills: deep-research, ralplan, ralph, triage, autopilot |
| [markoblogo/abvx-agent-skills](https://github.com/markoblogo/abvx-agent-skills) | production | Auditable coding skillpack (diffs, evidence, review) |
| [Lethe044/hermes-incident-commander](https://github.com/Lethe044/hermes-incident-commander) | beta | SRE detect / heal / learn on Hermes primitives |
| [Lethe044/hermes-life-os](https://github.com/Lethe044/hermes-life-os) | experimental | Personal OS + memory + cron patterns |
| [Yonkoo11/hermes-dojo](https://github.com/Yonkoo11/hermes-dojo) | beta | Monitor weak skills → self-evolve → report |
| [Hmbown/Wizards-of-the-Ghosts](https://github.com/Hmbown/Wizards-of-the-Ghosts) | experimental | Fantasy-themed dev ops skill pack |
| [Alexeyisme/hermes-spotify-skill](https://github.com/Alexeyisme/hermes-spotify-skill) | beta | Headless Linux / Pi Spotify control |
| [adnw-vinc/hermes-nextcloud](https://github.com/adnw-vinc/hermes-nextcloud) | beta | Nextcloud files / notes / cal / contacts bridge |
| [Lethe044/hermes-skill-marketplace](https://github.com/Lethe044/hermes-skill-marketplace) | experimental | Agent writes/tests/publishes skills |
| [beiyuii/personal-api-skill](https://github.com/beiyuii/personal-api-skill) | experimental | Obsidian vault → identity layer for agents |
| [Andrew-Girgis/microsoft-workspace-skill](https://github.com/Andrew-Girgis/microsoft-workspace-skill) | beta | Outlook / M365 Graph email+calendar skill |

---

## agentskills.io & cross-harness packs

These install on Hermes **and** often Claude Code / Cursor / OpenClaw / Codex.

| Project | Maturity | Why |
| --- | --- | --- |
| [mukul975/Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | production | 750+ MITRE-mapped security skills |
| [black-forest-labs/skills](https://github.com/black-forest-labs/skills) | production | Official FLUX image generation skills |
| [smartcontractkit/chainlink-agent-skills](https://github.com/smartcontractkit/chainlink-agent-skills) | production | Official Chainlink oracle / CCIP skills |
| [Agents365-ai/drawio-skill](https://github.com/Agents365-ai/drawio-skill) | production | draw.io from natural language |
| [ZeroPointRepo/youtube-skills](https://github.com/ZeroPointRepo/youtube-skills) | production | YouTube search + robust transcripts |
| [Infrasity-Labs/dev-gtm-claude-skills](https://github.com/Infrasity-Labs/dev-gtm-claude-skills) | production | SEO / GEO / developer marketing skills |
| [nowork-studio/NotFair](https://github.com/nowork-studio/NotFair) | production | 42 host-agnostic SEO, GEO, Google Ads, and Meta Ads skills; live account actions use approval-gated MCP connections |
| [CorpusIQ/corpusiq-docs](https://github.com/CorpusIQ/corpusiq-docs) | production | Business ops + many SaaS connectors via MCP |
| [longbridge/skills](https://github.com/longbridge/skills) | production | Markets / portfolio skills (multi-region) |
| [DougTrajano/pydantic-ai-skills](https://github.com/DougTrajano/pydantic-ai-skills) | production | Type-safe Pydantic AI + agentskills.io |
| [nexu-io/open-design](https://github.com/nexu-io/open-design) | production | Design system + media skills; Hermes via ACP |
| [runapi-ai/cli-skill](https://github.com/runapi-ai/cli-skill) | beta | Run AI image, video, music/audio, and model API jobs from CLI-capable agents |
| [Orkas-AI/Orkas-VideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) | beta | 14-skill video-production pack with editable `plan.json` workflows and source-installable CLI/MCP tooling |
| [Yarmoluk/cognify-skills](https://github.com/Yarmoluk/cognify-skills) | beta | CRM / invoicing / PM business ops |
| [tiann/execplan-skill](https://github.com/tiann/execplan-skill) | beta | Long-running task lifecycle / checkpoints |
| [ReinaMacCredy/maestro](https://github.com/ReinaMacCredy/maestro) | beta | Skill orchestration with planning + tracking |
| [armelhbobdad/bmad-module-skill-forge](https://github.com/armelhbobdad/bmad-module-skill-forge) | beta | Convert repos/docs into skills |
| [cablate/Agentic-MCP-Skill](https://github.com/cablate/Agentic-MCP-Skill) | beta | MCP client + agentskills validation |
| [Merit-Systems/agentcash-skills](https://github.com/Merit-Systems/agentcash-skills) | watch | Wallet-backed API access — **quarantine until dry-run + human spend gate** |
| [Xquik-dev/x-twitter-scraper](https://github.com/Xquik-dev/x-twitter-scraper) | beta | Large X/Twitter skill surface |
| [remoet-labs/agent-skills](https://github.com/remoet-labs/agent-skills) | production | Job search by tech stack + MCP |
| [Sequenzy/skills](https://github.com/Sequenzy/skills) | beta | Email marketing lifecycle skills |
| [resemble-ai/detect-skill](https://github.com/resemble-ai/detect-skill) | beta | Deepfake / media authenticity for agents |

---

## Visual production skills

Prompt-director and video `SKILL.md` packs. Keep the **discipline** (locks, density, pre-prompt checks); route the backend to the engine you already pay for.

| Project | Maturity | Why |
| --- | --- | --- |
| [remotion-dev/skills](https://github.com/remotion-dev/skills) | production | Official programmatic-video skills |
| [black-forest-labs/skills](https://github.com/black-forest-labs/skills) | production | Official FLUX stills |
| [Orkas-AI/Orkas-VideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) | beta | 14-skill video pack with `plan.json` workflows |
| [smixs/visual-skills](https://github.com/smixs/visual-skills) | production | Image + video toolkit; Hermes-compatible |
| [Gregory-Esman/ai-film-pipeline](https://github.com/Gregory-Esman/ai-film-pipeline) | production | Film OS: director + worldbuilder + video QA |
| [nexu-io/open-design](https://github.com/nexu-io/open-design) | production | Design system + media; Hermes via ACP |

Spoke: [awesome-motion-design-agent-skills](https://github.com/frankxai/awesome-motion-design-agent-skills) · [awesome-design-agent-skills](https://github.com/frankxai/awesome-design-agent-skills)

## Domain skill packs

| Project | Domain |
| --- | --- |
| [setasoma/mycodo-hermes-skill](https://github.com/setasoma/mycodo-hermes-skill) | IoT mushroom cultivation |
| [bbolinger/snapmaker-u1-toolkit](https://github.com/bbolinger/snapmaker-u1-toolkit) | 3D printer automation |
| [currentslab/news-api-skills](https://github.com/currentslab/news-api-skills) | News search/read skills |
| [internet-court/internet-court-skill](https://github.com/internet-court/internet-court-skill) | Agent commerce / escrow patterns |
| [longsizhuo/openInvest](https://github.com/longsizhuo/openInvest) | Investment research (not advice) |
| [avansaber/erpclaw](https://github.com/avansaber/erpclaw) | ERP + agent action layer |
| [wordbricks skills / onequery-cli](https://github.com/wordbricks/skills/tree/main/skills/onequery-cli) | Governed read-only SQL for agents |

---

## Skill factories & evolution

| Project | Why |
| --- | --- |
| Built-in Hermes skill creation + curator | Official closed loop — see [skills docs](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills) |
| [Romanescu11/hermes-skill-factory](https://github.com/Romanescu11/hermes-skill-factory) | Turn sessions into reusable skills |
| [AMAP-ML/SkillClaw](https://github.com/AMAP-ML/SkillClaw) | Evolve/dedupe libraries from session data; native Hermes paths |
| [NousResearch/hermes-agent-self-evolution](https://github.com/NousResearch/hermes-agent-self-evolution) | Research: DSPy + GEPA evolution |
| [Yonkoo11/hermes-dojo](https://github.com/Yonkoo11/hermes-dojo) | Find weak skills and improve them |
| [Lethe044/hermes-skill-marketplace](https://github.com/Lethe044/hermes-skill-marketplace) | Publish pipeline experiments |

---

## Related tools (skills-adjacent)

Not pure `SKILL.md` packs, but skill operators use them constantly:

| Project | Role |
| --- | --- |
| [outsourc-e/hermes-workspace](https://github.com/outsourc-e/hermes-workspace) | GUI with skills manager |
| [builderz-labs/mission-control](https://github.com/builderz-labs/mission-control) | Fleet dispatch + cost |
| [luoyuctl/agenttrace](https://github.com/luoyuctl/agenttrace) | Session audit skill companion |
| [fkiene/llmtrim](https://github.com/fkiene/llmtrim) | Trim tool schemas before model calls |
| [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) | Full agents/UI/deploy list |

---

## August 2026 research additions

Resolved through GitHub repository metadata on **2026-08-30** (and the 2026-08-06 pulse retained where still accurate). Stars are a dated discovery signal, not an install rank.

| Project | Pulse snapshot | Why it belongs here | Caveat |
| --- | --- | --- | --- |
| [Anthropic skills](https://github.com/anthropics/skills) | ~173k★ · `NOASSERTION` | Official examples including skill-creator, xlsx, frontend/design. | Install **named** skills; inspect license. |
| [Obra Superpowers](https://github.com/obra/superpowers) | ~280k★ · MIT | TDD, debug, review methodology operators actually run. | Methodology, not a second OS. |
| [gstack](https://github.com/garrytan/gstack) | ~130k★ · MIT | Product/design/eng/QA/browser workflows. | Opinionated; adapt, don't clone blindly. |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | ~91k★ · MIT | Production engineering skills. | Per-repo fit required. |
| [NVIDIA SkillSpector](https://github.com/NVIDIA/SkillSpector) | ~15k★ · Apache-2.0 | Scanner for injection, exfil, supply-chain in skills. | Signal, not a warranty. |
| [agentskills/agentskills](https://github.com/agentskills/agentskills) | ~25k★ · Apache-2.0 | Portable skill-package spec. | Spec, not a skill dump. |
| [google/skills](https://github.com/google/skills) | Apache-2.0 | Vendor skills for Google products. | Product data boundaries. |
| [huggingface/skills](https://github.com/huggingface/skills) | Apache-2.0 | Official HF ecosystem skills. | Token/model requirements. |
| [remotion-dev/skills](https://github.com/remotion-dev/skills) | `NOASSERTION` | Programmatic video. | Review render deps + license. |
| [mattpocock/skills](https://github.com/mattpocock/skills) | MIT | Small composable engineering skills. | Assess each skill. |
| [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | ~26k★ | Crash-proof plans across compaction. | Inspect current license. |
| [blader/humanizer](https://github.com/blader/humanizer) | ~39k★ | Strip generic AI prose. | Writing aid, not a truth gate. |
| [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) | ~38k★ | Validated science skills + databases. | Domain-specific; do not bulk-install. |
| [github/awesome-copilot](https://github.com/github/awesome-copilot) | ~38k★ | Copilot agents/skills/instructions. | GitHub Copilot surface. |
| [bergside/awesome-design-skills](https://github.com/bergside/awesome-design-skills) | ~2.6k★ | Ranked DESIGN.md / SKILL.md for UI agents. | Directory + ranked files; still read source. |
| [gamedev-skills/awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) | ~0.8k★ | 67 engine skills + router. | Install **router + one engine**, not all 67. |
| [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills) | MIT | Obsidian-format agent workflows. | Vault permission review. |

## Directories, not installs

Use these to **find** primary sources. Do not copy the whole tree into a live agent.

| Directory | Pulse | Use as |
| --- | --- | --- |
| [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | ~74k★ | Claude skill index |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | ~53k★ | Claude Code ecosystem index |
| [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | ~33k★ | Cross-harness discovery |
| [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) | ~46k★ | 2,000+ catalog — curate, never bulk-install |
| [futantan/agent-skills.md](https://github.com/futantan/agent-skills.md) | ~0.3k★ | Discovery UI |
| [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) | ~52k★ | **Quarantine** (OpenClaw-adjacent mass dump) |

---

## 6-Pillar curation lens

This lens describes how we evaluate an operator skill after web-first evidence, repository ownership, license posture, and install path—not instead of them.

```mermaid
mindmap
  root((Hermes skill curation))
    Strategy
      operator outcome
      scope and fit
    Governance
      provenance
      license review
    Talent
      human-agent collaboration
      reusable practice
    Technology
      SKILL.md packages
      MCP and harness compatibility
    Data
      source-backed research pulses
      update evidence
    Ethics
      least privilege
      transparent limitations
```

---

## Explore the Full FrankX Awesome Ecosystem (17 lists) (optional)

These companion lists are optional follow-on reading—not a substitute for the independent catalog above.

- [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents) · [awesome-manifestation-skills](https://github.com/frankxai/awesome-manifestation-skills) · [awesome-ai-coe](https://github.com/frankxai/awesome-ai-coe)
- [awesome-agentic-income](https://github.com/frankxai/awesome-agentic-income) · [awesome-investor-agent-skills](https://github.com/frankxai/awesome-investor-agent-skills) · [awesome-design-agent-skills](https://github.com/frankxai/awesome-design-agent-skills) · [awesome-agent-operating-systems](https://github.com/frankxai/awesome-agent-operating-systems)
- [awesome-hermes-agent-skills](https://github.com/frankxai/awesome-hermes-agent-skills) · [awesome-gamification-agent-skills](https://github.com/frankxai/awesome-gamification-agent-skills) · [awesome-wealth-agent-skills](https://github.com/frankxai/awesome-wealth-agent-skills) · [awesome-mind-agent-skills](https://github.com/frankxai/awesome-mind-agent-skills)
- [awesome-cosmos-ai-agents](https://github.com/frankxai/awesome-cosmos-ai-agents) · [awesome-automation-agent-skills](https://github.com/frankxai/awesome-automation-agent-skills) · [awesome-payment-agent-skills](https://github.com/frankxai/awesome-payment-agent-skills) · [awesome-motion-design-agent-skills](https://github.com/frankxai/awesome-motion-design-agent-skills) · [awesome-music-agent-skills](https://github.com/frankxai/awesome-music-agent-skills)

---

## Maintained in this repo (optional)

Small **open-core** packs we ship for free. These are **not** “the list” — the list above is the list.

| Pack | Description | Path |
| --- | --- | --- |
| **coding-agents-superpack** | Multi-CLI discovery, structured prompts, council handoffs (sanitized) | [`skills/coding-agents-superpack`](./skills/coding-agents-superpack/SKILL.md) |
| **todo-discipline** | Task list must match reality before “done” | [`skills/todo-discipline`](./skills/todo-discipline/SKILL.md) |

```bash
git clone https://github.com/frankxai/awesome-hermes-agent-skills.git
cp -R awesome-hermes-agent-skills/skills/todo-discipline ~/.hermes/skills/
```

**Rule:** stranger can run it with no private secrets → free. Brand/production CoE kits stay gated elsewhere.

---

## Skill Portfolio OS

How we classify free vs gated vs product (ops for maintainers of *this* tree):

→ [`docs/skill-portfolio-os/`](./docs/skill-portfolio-os/)

Especially: [CLASSIFICATION.md](./docs/skill-portfolio-os/CLASSIFICATION.md) · [PUBLISH-PLAYBOOK.md](./docs/skill-portfolio-os/PUBLISH-PLAYBOOK.md) · [STORAGE-TAXONOMY.md](./docs/skill-portfolio-os/STORAGE-TAXONOMY.md)

---

## Contributing

- Add **web** skills with: link, one-line why, maturity, and that it actually has a `SKILL.md` / install path.  
- Prefer PRs that improve discovery of **others'** work.  
- Own packs must stay secret-free and portable.  
- Agent/UI/deploy entries → [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents).  
- See [CONTRIBUTING.md](./CONTRIBUTING.md) · [GETTING_STARTED.md](./GETTING_STARTED.md)

---

## License

[MIT](./LICENSE)

---

<p align="center">
  <sub>Curated by <a href="https://github.com/frankxai">frankxai</a>
  · Ecosystem also: <a href="https://github.com/0xNyk/awesome-hermes-agent">0xNyk</a> · <a href="https://github.com/SamurAIGPT/awesome-hermes-agent">SamurAIGPT</a>
  · Agents companion: <a href="https://github.com/frankxai/awesome-hermes-agents">awesome-hermes-agents</a>
  · Pulse: <strong>2026-08-30</strong></sub>
</p>
