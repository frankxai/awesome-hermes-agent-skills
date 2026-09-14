# Tier Registry (living)

**Updated:** 2026-07-15  
**Source of truth for decisions:** CLASSIFICATION.md  
**Runtime count (approx):** 153 skills

## Pins (runtime)

| Skill | Tier | Notes |
|-------|------|-------|
| windows-phone-link-search-safety | T0 | Host critical; sanitized T1 project-scoped-search companion drafted 2026-09-14 |
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
| P1 | Provider-neutral AI usage telemetry foundation | awesome-hermes-agent-skills | **in progress** — sanitized T1 reference added 2026-09-14; implementation gated on current parser, license, and redaction evidence |
| P1 | hermes-agent-skill-authoring (already official-aligned) | keep / mirror | ok |
| P2 | process suite (plan, TDD, debug, spike) | ACOS | partial upstream |
| P2 | architecture-diagram + excalidraw packs | design awesome | later |

## Absorb-then-delete / merge candidates

| Skill | Action | Status |
|-------|--------|--------|
| mcr-multi-cli-router | Re-absorb into coding-agents routing section; then replace legacy full copy with compatibility redirect | **reopened** 2026-09-14 — runtime audit found a full legacy skill, not a redirect stub |
| agy-mcr-orchestrator | Re-absorb into coding-agents + agy-cli; then replace legacy full copy with compatibility redirect | **reopened** 2026-09-14 — runtime audit found a full legacy skill, not a redirect stub |
| si-starlight-intelligence | Re-absorb into starlight-queen; then replace legacy full copy with compatibility redirect | **reopened** 2026-09-14 — runtime audit found a full legacy skill, not a redirect stub |
| build-in-public / daily-building-in-public | Re-absorb into `build-in-public`; then replace the legacy page with a compatibility redirect | **reopened** 2026-09-14 — active target profile retains a divergent full legacy page (checksum differs from `build-in-public`), not a redirect stub |
| ai-agent-token-tracking / starlight-token-tracker | Extract a provider-neutral usage-telemetry T1 draft; do not export the branded runtime root skill or create an alias yet | **re-scoped** 2026-09-14 — source review complete; generic draft needs current-tool and license verification |

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
