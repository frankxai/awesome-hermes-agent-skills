# Where things live — Starlight storage taxonomy (binding)

**Updated:** 2026-07-15  
**Why this exists:** Agents wrote durable Skill Portfolio OS under `starlight/ops/` (estate control plane). That path is **not** a reliable GitHub product SoT. Durable systems must live in **`starlight/repos/<git-repo>`** with a remote.

## Layer model (memorize)

| Layer | Path | GitHub? | What belongs here | What does NOT |
|-------|------|---------|-------------------|---------------|
| **L0 Runtime** | `%LOCALAPPDATA%\hermes\` · `~\.starlight\` | No | Live skills, memory, sessions, crons, locks, queues | Product docs, free packs, strategy SSOT |
| **L1 Estate control plane** | `C:\Users\frank\starlight\` (not under repos) | Fragile / often push-disabled | AGENTS.md, WORKSPACE_MAP, queen reports, **thin pointers**, FLEET index | Full operating systems, skill packs, CoE kits |
| **L2 Repo estate (SSOT)** | `C:\Users\frank\starlight\repos\<repo>\` | **Yes — required** | All durable docs, code, public free packs, private strategy when that repo is private | Random new top-level home folders |
| **L3 Quarantine / litter** | `universe\`, home one-offs | No | Scratch only | Never treat as canon |

## Rules

1. **If it must survive, sync, PR, or be reused by other machines → L2 git repo.**  
2. **If it is only “how this machine is wired today” → L0 runtime + short L1 pointer.**  
3. **L1 `ops/` may index and point; it must not be the only copy of a system.**  
4. Prefer **existing frankxai repo** over inventing a new one.  
5. Public open-core vs private product → **different repos or different paths** (see skill portfolio).

## Skill Portfolio OS placement (corrected)

| Content | Correct home | Remote |
|---------|--------------|--------|
| Open-core portfolio OS (classification, maintenance, self-learn, free funnel, publish playbook) | `starlight/repos/awesome-hermes-agent-skills/docs/skill-portfolio-os/` | `frankxai/awesome-hermes-agent-skills` |
| Free skill packs | `…/skills/*` same repo | same |
| Private CoE kit SKU / pricing / empire product | `starlight/repos/FrankX/docs/products/` | `frankxai/FrankX` (private) |
| Hermes loadable skill | `%LOCALAPPDATA%\hermes\skills\…\skill-portfolio-ops` | N/A (runtime; may mirror process skill later) |
| Estate pointer only | `starlight/ops/skill-portfolio-os/README.md` → redirects to L2 | Not SoT |

## Other common systems (map)

| System | Prefer |
|--------|--------|
| Workspace bootstrap doctrine | agent-config + Hermes skill + L1 ops index pointer |
| Free Claude packs | `claude-skills-library` |
| Creator OS open-core | `agentic-creator-os` |
| SIS substrate | `Starlight-Intelligence-System` |
| Private strategy | `FrankX`, `gencreator.ai` |
| Queen evidence | `starlight/queen/reports/` (local ops; promote summaries into repo when durable) |

## Anti-patterns (observed)

| Bad | Why | Fix |
|-----|-----|-----|
| Full OS only under `starlight/ops/` | Not pushed; agents treat as “done”; multi-machine drift | Copy to L2 + push; leave redirect |
| Full OS only under `universe/` | Quarantined | Delete/redirect |
| Dump entire Hermes skills tree to public | Secrets, stubs, host PII | Promote sanitized packs only |
| New `C:\Users\frank\my-ops\` | Home litter | Use `starlight/repos/<repo>` |
| Writing product into estate root git | Push disabled / mixed history | Child repo worktree |

## Decision tree

```
Is this a live agent skill the model loads?
  → Hermes runtime skills/ (L0). If portable free pack, ALSO promote to L2 public skills/.

Is this durable process/product documentation?
  → L2 starlight/repos/<existing or new frankxai repo> + push.

Is this machine-only wiring (cron workdir, fleet map)?
  → L0/L1 index; pointer to L2 for the “how we operate” docs.

Is this a one-session report?
  → queen/reports/; promote to L2 if still true next week.
```

## This correction

Skill Portfolio OS was first written to L1 `ops/` for speed. **Corrected:** primary SoT = **awesome-hermes-agent-skills** `docs/skill-portfolio-os/` (GitHub). Private SKU remains FrankX. L1 holds redirect only.
