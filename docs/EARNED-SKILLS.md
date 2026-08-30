# Earned skills index

Start here. These are **structured workflows** people actually run — not a 500-skill dump.

Review state: `reviewed` against public GitHub README + license on **2026-08-30**. Not sandbox-`tested` unless noted.

## Operator core (install 5–7, not 500)

| Skill / pack | Job | License snapshot | Why it earns a slot |
| --- | --- | --- | --- |
| [agentskills/agentskills](https://github.com/agentskills/agentskills) | Portable `SKILL.md` spec | Apache-2.0 · ~24.9k★ | The format Hermes, Claude Code, Codex, Cursor, and Gemini CLI share |
| [anthropics/skills](https://github.com/anthropics/skills) | Official examples (`xlsx`, `docx`, `pdf`, `skill-creator`, frontend/design) | inspect `LICENSE` · ~173k★ | Vendor source of truth; install **named** skills, not the whole tree blindly |
| [obra/superpowers](https://github.com/obra/superpowers) | TDD, brainstorm, systematic debug, review, shipping | MIT · ~280k★ | Methodology operators actually follow; closest thing to a junior-dev playbook |
| [garrytan/gstack](https://github.com/garrytan/gstack) | CEO/design/eng/QA/browser workflows | MIT · ~130k★ | Product + design + verification loops in one opinionated CLI |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | Production engineering skills | MIT · ~91k★ | Tight, named jobs for coding agents |
| [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) | Scan skills for injection, exfil, supply-chain | Apache-2.0 · ~15k★ | Treat install like installing software |
| [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | Crash-proof plans across compaction | MIT · ~26k★ | Long-running work that survives `/clear` |

If you already have the core seven, add [mattpocock/skills](https://github.com/mattpocock/skills) (MIT) for small composable TypeScript/engineering skills — do not treat it as a required eighth.

## FrankX free packs (optional, last)

Portable, secret-free, listed last on purpose:

| Pack | Job | Path |
| --- | --- | --- |
| `todo-discipline` | Task list must match reality before “done” | [`skills/todo-discipline`](../skills/todo-discipline/SKILL.md) |
| `coding-agents-superpack` | Multi-CLI discovery and handoffs (sanitized) | [`skills/coding-agents-superpack`](../skills/coding-agents-superpack/SKILL.md) |

## Domain map (spoke lists)

Each spoke should stay useful if every `frankxai/*` link is removed.

| Domain | Spoke | Start with (third-party) |
| --- | --- | --- |
| Coding / agent OS | [awesome-agent-operating-systems](https://github.com/frankxai/awesome-agent-operating-systems) | Superpowers, gstack, Anthropic skills, Hermes docs |
| Design / UI | [awesome-design-agent-skills](https://github.com/frankxai/awesome-design-agent-skills) | [bergside/awesome-design-skills](https://github.com/bergside/awesome-design-skills), [nexu-io/open-design](https://github.com/nexu-io/open-design), Anthropic frontend/canvas skills |
| Motion / video | [awesome-motion-design-agent-skills](https://github.com/frankxai/awesome-motion-design-agent-skills) | [remotion-dev/skills](https://github.com/remotion-dev/skills), [Orkas-AI/Orkas-VideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) |
| Animation | [awesome-motion-design-agent-skills](https://github.com/frankxai/awesome-motion-design-agent-skills) | Blender, Remotion, Motion |
| Game | [awesome-gamedev-agent-skills](https://github.com/frankxai/awesome-gamedev-agent-skills) | Upstream [gamedev-skills/awesome-gamedev-agent-skills](https://github.com/gamedev-skills/awesome-gamedev-agent-skills) — **router + one engine**, not all 67 |
| Music | [awesome-music-agent-skills](https://github.com/frankxai/awesome-music-agent-skills) | Audiocraft, librosa, Remotion for canvas |
| Payments | [awesome-payment-agent-skills](https://github.com/frankxai/awesome-payment-agent-skills) | AP2, x402, Stripe MCP — **mandate before settle** |
| Wealth / research | [awesome-wealth-agent-skills](https://github.com/frankxai/awesome-wealth-agent-skills) | OpenBB, Qlib — not advice |
| Investor research | [awesome-investor-agent-skills](https://github.com/frankxai/awesome-investor-agent-skills) | OpenBB, longbridge/skills — simulation/research only |
| Automation | [awesome-automation-agent-skills](https://github.com/frankxai/awesome-automation-agent-skills) | MCP registry, n8n, Prefect |
| Science | (hub row) | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| Copilot | (hub row) | [github/awesome-copilot](https://github.com/github/awesome-copilot) |
| Writing | (hub row) | [blader/humanizer](https://github.com/blader/humanizer) |

## Directories, not installs

Use these to **find** primary sources. Do not bulk-install:

| Directory | Why it is a directory |
| --- | --- |
| [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | Large Claude skill index |
| [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | 1,000+ cross-harness listings |
| [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) | 2,000+ catalog / control plane |
| [hesreallyhim/awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) | Claude Code ecosystem index |
| [futantan/agent-skills.md](https://github.com/futantan/agent-skills.md) | Discovery UI |

**Quarantine by default:** [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) (OpenClaw-adjacent mass dump).

## X pulse (public posts, 2026-08-30)

What operators repeated — used as leads, then checked on GitHub:

- Skills that do **one named job**, source-readable, updated in 90 days ([skillsboard.sh criteria](https://www.skillsboard.sh/best-claude-skills)).
- Superpowers + Anthropic official skills + gstack as the actual daily stack.
- NVIDIA SkillSpector as the missing install gate (“skills are becoming npm for behavior”).
- Engagement-bait “53 skills free if you RT” posts are **not** sources.

## What we will not list as a default OS

Everything Claude Code / ECC-style mega-packs, 1,900-skill bots, and anonymous marketplace ZIPs. If a methodology is needed, Superpowers + gstack + this spec already cover it.
