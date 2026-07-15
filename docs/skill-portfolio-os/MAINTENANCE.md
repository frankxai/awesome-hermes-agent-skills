# Skill Repo Maintenance (Scale Ops)

## Dual-tree model (always)

```
┌────────────────────────────┐     refresh      ┌──────────────────────────────┐
│ OFFICIAL BUNDLE (read)     │ ───────────────► │ ACTIVE RUNTIME (load)        │
│ hermes-agent/skills/       │   + overlays     │ %LOCALAPPDATA%/hermes/skills │
└────────────────────────────┘                  └──────────────┬───────────────┘
                                                               │ promote
                                                               ▼
┌────────────────────────────┐     package      ┌──────────────────────────────┐
│ PRIVATE STRATEGY HUBS      │ ◄── strategy ──  │ PUBLIC SKILL REPOS (T1/T2)   │
│ FrankX, gencreator.ai      │                  │ ACOS, SIS, awesome-*, libs   │
└────────────────────────────┘                  └──────────────────────────────┘
```

| Tree | Path / repo | Write policy |
|------|-------------|--------------|
| **Runtime** | `AppData\Local\hermes\skills\` | Daily: `skill_manage` patch/create; pin critical |
| **Official** | `AppData\Local\hermes\hermes-agent\skills\` | **Do not edit as SoT**; re-copy leaves after Hermes update; re-apply overlays |
| **Public** | frankxai public skill/OS repos | Sanitized T1/T2 only; MIT; CI link check |
| **Private** | FrankX, gencreator.ai, vaults | T3/T4 strategy + premium sources |

## Ownership matrix

| Skill class | Owner role | Cadence |
|-------------|------------|---------|
| Official leaves (`claude-code`, `codex`, `opencode`, `hermes-agent`) | Tech / Technology pillar | On every Hermes update |
| Frank umbrellas (`coding-agents`, `starlight-queen`) | Queen / Technology | Weekly absorb |
| Process (`todo-discipline`, plan, TDD) | Governance + Technology | After every failure mode |
| Host safety (Windows path ban) | Governance (pinned) | Immediate on new trigger |
| Creative / brand packs | Arcanea + Design | Per campaign |
| Awesome lists | Growth + Research | Monthly pulse (existing skill) |
| Premium vault content | Product | Release train |

## Weekly ops ritual (30–60 min)

1. **Curator status** — `hermes curator status` (agent-created skills)  
2. **Pin check** — path-safety, todo-discipline, coding-agents, hermes-agent present  
3. **Stale scan** — thin v0.1 stubs: absorb or delete  
4. **Official delta** — if Hermes updated, diff bundled leaves vs active; rebase overlays  
5. **Promote queue** — any session patch that is generic → sanitize → public PR  
6. **Gate queue** — production-only improvements → vault / private  
7. **Registry update** — `registry/TIER-REGISTRY.md`  
8. **Self-learning log** — append week’s absorbs to `SELF-LEARNING-LOOP.md` log section  

## Monthly ops ritual

1. Awesome-list research pulse (`awesome-list-maintenance`)  
2. Arena / eval pulse if multi-llm-arena used  
3. Product free/paid boundary review (PRODUCT-MAP)  
4. Skill count budget: descriptions cost tokens — archive zero-use agent skills  
5. Cross-repo link health on public skill libraries  

## Official leaf refresh procedure

```bash
# After hermes update — example for claude-code
BUNDLED="$LOCALAPPDATA/hermes/hermes-agent/skills/autonomous-ai-agents/claude-code/SKILL.md"
ACTIVE="$LOCALAPPDATA/hermes/skills/autonomous-ai-agents/claude-code/SKILL.md"
OVERLAY="$LOCALAPPDATA/hermes/skills/autonomous-ai-agents/claude-code/references/frank-overlay.md"

# 1. Backup active
cp "$ACTIVE" "$ACTIVE.bak.$(date +%Y%m%d)"

# 2. Diff
diff -u "$BUNDLED" "$ACTIVE" | head -100

# 3. Prefer: copy official body, re-append overlay section from frank-overlay.md
# 4. Keep Windows path ban injection in overlay only
# 5. Verify with skill_view after new session
```

**Overlay contract:** Official body = flags/modes/dialogs. Overlay = Frank preferences, path ban injection, hybrid massive action, brand fleet notes.

## Local skill authoring

| Action | Tool |
|--------|------|
| New personal skill | `skill_manage(create)` → runtime tree |
| Patch after failure | `skill_manage(patch)` same session |
| In-repo (ACOS/SIS/public) | `write_file` in clone + git commit (not skill_manage create) |
| Quality bar | Load `hermes-agent-skill-authoring` |

## Pin list (non-negotiable)

```text
windows-phone-link-search-safety
todo-discipline
coding-agents
hermes-agent
skill-portfolio-ops
```

Optional pins: `claude-code`, `empire-planning` (private-heavy — pin only if needed).

## Windows / Phone Link (ops)

- **Never** recursive search from `C:\`, home, `This PC` on Frank host.  
- Inject ban into every `delegate_task` and coding-CLI prompt.  
- Free community version: “prefer project-scoped search roots; avoid home recursion on Windows multi-device setups.”  

## Multi-repo packaging map

| Public repo | What it maintains |
|-------------|-------------------|
| [awesome-hermes-agent-skills](https://github.com/frankxai/awesome-hermes-agent-skills) | Seed + curated Hermes skill packs (T1) |
| [claude-skills-library](https://github.com/frankxai/claude-skills-library) | Claude-oriented professional packs (T1) |
| [agentic-creator-os](https://github.com/frankxai/agentic-creator-os) | Open-core creator OS skills/commands (T2) |
| [Starlight-Intelligence-System](https://github.com/frankxai/Starlight-Intelligence-System) | Substrate + multi-agent standards (T2) |
| [workflow-tier-plugin](https://github.com/frankxai/workflow-tier-plugin) | Portable multi-agent workflows MIT (T1/T2) |
| [starlight-automation-agent-skills](https://github.com/frankxai/starlight-automation-agent-skills) | Automation skill pack (T1/T2) |
| [sentinel-swarm-agent-skills](https://github.com/frankxai/sentinel-swarm-agent-skills) | Sentinel skills (T1/T2) |
| awesome-* lists | Discovery surface, not full skill bodies |

| Private | What it maintains |
|---------|-------------------|
| FrankX | Empire strategy, deep plans, classification decisions |
| gencreator.ai | Product/CoE private |
| realityarchitect-vault | Paid production systems |
| Hermes runtime + profiles | Live skills, memory, cron |

## Quality gates before any public push

1. Classification test (CLASSIFICATION.md)  
2. Sanitizer checklist (PUBLISH-PLAYBOOK.md)  
3. Frontmatter valid; description ≤ 1024  
4. No secrets (`gitleaks` / manual scan)  
5. README install path for Hermes + Claude Code  
6. License file (MIT default for T1)  
7. Cross-link to ecosystem without leaking private URLs  

## Failure modes & fixes

| Failure | Fix |
|---------|-----|
| Skills sediment / god skills | Split references; prune; umbrella routes only |
| Official leaf fork forever | Overlay pattern + refresh ritual |
| Public/private drift | Single promote pipeline; registry version |
| 150 skills kill tokens | Archive unused; shorter descriptions; curator |
| Agent claims done, todos open | todo-discipline pin + read-verify |
| Subagents search home | Path ban in every prompt; skill-portfolio-ops |
