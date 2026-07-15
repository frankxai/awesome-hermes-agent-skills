# Publish Playbook — Package & Share Safely

## Goal

Ship **high-signal free skills** to the community while protecting private/gated moat and never leaking secrets.

## Channels

| Channel | Use for |
|---------|---------|
| [awesome-hermes-agent-skills](https://github.com/frankxai/awesome-hermes-agent-skills) | Hermes-native SKILL.md packs |
| [claude-skills-library](https://github.com/frankxai/claude-skills-library) | Claude Code / Claude AI packs |
| [agentic-creator-os](https://github.com/frankxai/agentic-creator-os) | Multi-harness creator OS skills |
| [Starlight-Intelligence-System](https://github.com/frankxai/Starlight-Intelligence-System) | Substrate / multi-agent standards |
| [workflow-tier-plugin](https://github.com/frankxai/workflow-tier-plugin) | Portable workflow plugins |
| Domain awesome-* | Discovery pointers (not full private bodies) |
| Hermes Skills Hub | When pack is hub-ready (`hermes skills publish`) |
| Upstream Nous | Only general leaf improvements (PRs), not Frank OS |

## Sanitizer checklist (mandatory)

Before any public commit:

- [ ] Strip `C:\Users\frank`, OnePlus, Phone Link device specifics  
- [ ] Strip API keys, tokens, webhooks, private emails  
- [ ] Strip private repo names that reveal unreleased strategy (or replace with placeholders)  
- [ ] Strip personal health/finance/client data  
- [ ] Replace Frank-only brand internal codenames if needed for clarity  
- [ ] Genericize “user preference” into optional configuration  
- [ ] Add `When to use` / `Don't use`  
- [ ] Add Verification checklist  
- [ ] License MIT (or match target repo)  
- [ ] Install instructions for Hermes and/or Claude Code  
- [ ] Version bump + changelog line  

## Sanitize pattern (coding-agents example)

| Keep free | Remove / rewrite |
|-----------|------------------|
| Discovery `which` + doctor | Hard-coded Frank paths |
| Structured prompt template | Multi-brand ECOSYSTEM private wiring |
| Model Council board pattern | Machine names c940/yogabook |
| Comparison temp-git recipes | Phone Link incident narrative |
| Hybrid “direct + CLI” principle | Personal “not codex for now” preference as law |

## Package layout (public pack)

```text
skill-name/
  SKILL.md
  LICENSE
  README.md          # human install
  references/        # optional progressive disclosure
  templates/         # optional
  scripts/           # optional
```

Frontmatter:

```yaml
---
name: skill-name
description: Use when <trigger>. <behavior>.
version: 1.0.0
author: Frank Riemer / GenCreator
license: MIT
metadata:
  hermes:
    tags: [...]
    related_skills: [...]
    provenance: frankx-public
    tier: free
---
```

## Promote pipeline (ops)

1. Mark item in `registry/PROMOTE-QUEUE.md`  
2. Copy skill to worktree under public repo  
3. Run sanitizer checklist  
4. Validate frontmatter (authoring skill)  
5. PR or direct commit on public repo  
6. Link from relevant awesome-*  
7. Optional: `hermes skills publish` if hub path ready  
8. Log in SELF-LEARNING-LOOP absorb log  

## Do not publish

- Full runtime dump of `~/.hermes/skills`  
- T0 host skills as-is  
- T3/T4 empire/finance/health  
- Thin v0.1 stubs without verification  
- Skills that only work with private MCP credentials undocumented  

## Community positioning (copy)

> Portable agent skills and workflows from GenCreator / Starlight / Arcanea — open-core excellence you can run locally. Production CoE kits and brand systems available separately.

## Attribution

- Credit Nous Hermes for platform skills patterns.  
- Credit upstream CLI vendors (Anthropic, OpenAI, etc.) for tool behavior.  
- Frank/GenCreator for orchestration OS and free packs.  
