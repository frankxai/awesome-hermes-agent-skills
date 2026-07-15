# Tier Registry (living)

**Updated:** 2026-07-15  
**Source of truth for decisions:** CLASSIFICATION.md  
**Runtime count (approx):** 153 skills

## Pins (runtime)

| Skill | Tier | Notes |
|-------|------|-------|
| windows-phone-link-search-safety | T0 | Host critical |
| todo-discipline | T0/T1 | Core free-exportable |
| coding-agents | T4 + T1 export | Umbrella |
| hermes-agent | Official T1 | Refreshable |
| skill-portfolio-ops | T4 process / T1 templates | This OS |

## Free export priority queue (next)

| Priority | Skill / pack | Target repo | Status |
|----------|--------------|-------------|--------|
| P0 | coding-agents **sanitized** Superpack | awesome-hermes-agent-skills | **shipped** 2026-07-15 |
| P0 | todo-discipline generic | claude-skills-library + awesome-hermes-agent-skills | **shipped** (AHAS main; CSL PR #21) |
| P1 | Model Council reference only | starlight-swarm / ACOS | queued |
| P1 | hermes-agent-skill-authoring (already official-aligned) | keep / mirror | ok |
| P2 | process suite (plan, TDD, debug, spike) | ACOS | partial upstream |
| P2 | architecture-diagram + excalidraw packs | design awesome | later |

## Absorb-then-delete / merge candidates

| Skill | Action | Status |
|-------|--------|--------|
| mcr-multi-cli-router | Absorb into coding-agents routing section | **done** 2026-07-15 → redirect stub |
| agy-mcr-orchestrator | Absorb into coding-agents + agy-cli | **done** → redirect stub |
| si-starlight-intelligence | Absorb into starlight-queen | **done** → redirect stub |
| build-in-public / daily-building-in-public | Merge one | pending |
| ai-agent-token-tracking / starlight-token-tracker | Merge umbrella + alias | pending |

## Gated product sources (do not free)

| Skill / system | Product line |
|----------------|--------------|
| 6pillar-guardian-factory | GenCreator CoE kit |
| gencreator-swarm-evolver | CoE / service |
| brand-image-system full | Brand packs |
| creative-asset-management | Creator OS premium |
| velora personal seams | Velora product |
| arcanea-business-operator | Arcanea B2B |
| empire-planning deep | Advisory private |
| realityarchitect-vault | Paid vault |

## Official leaves (refreshable)

| Skill | Bundle | Active overlay? |
|-------|--------|-----------------|
| claude-code | yes | yes (Frank hybrid + path ban) |
| codex | yes | check |
| opencode | yes | check |
| hermes-agent | yes | Windows quirks section ok |

## Machine-private (never public as-is)

- starlight-queen-c940  
- starlight-queen-yogabook  
- swarm-comms-protocol (if contains private channels) — sanitize first  

## Registry ops

After every promote/absorb: update this file + PROMOTE-QUEUE.md.  
