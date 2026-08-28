# Self-Learning Loop (Absorb → Improve → Promote)

Self-learning is **not** optional. Every hard session must leave the system smarter. Hermes already supports skills as procedural memory; this OS makes the loop **explicit, tier-aware, and scalable**.

## The loop (tight)

```
RUN WORK
  → HIT FRICTION / WIN / CORRECTION
    → CAPTURE (failure mode, recipe, decision)
      → ABSORB (patch skill / new reference / new skill)
        → CLASSIFY (T0–T5)
          → PROMOTE (free) | GATE (premium) | KEEP (private)
            → VERIFY (checklist + next-run use)
              → LOG (this file + optional memory one-liner)
```

## When absorb is mandatory

| Trigger | Minimum absorb |
|---------|----------------|
| Same error twice | Pitfall + fix in skill |
| User correction of preference | Memory (durable) + skill if procedural |
| New CLI flag / version break | Leaf skill patch |
| Successful multi-step workflow (5+ tools) | Skill or reference |
| Cron/headless failure | todo-discipline / cron reference |
| Phone Link or host incident | path-safety skill immediately |
| Great multi-agent pattern | coding-agents or agentic-orchestration |
| Product boundary decision | CLASSIFICATION + PRODUCT-MAP |

## Session end protocol (agents)

Before any “work complete” (with todo-discipline):

1. List **what we learned** (3 bullets max if none).  
2. For each learning: **patch** skill OR **write** reference OR **create** skill.  
3. Classify promote path: free / gated / private.  
4. If free-worthy: open item in promote queue (`registry/PROMOTE-QUEUE.md`).  
5. Update todos merge+read.  

## Absorb targets by learning type

| Learning type | Write to | Tier default |
|---------------|----------|--------------|
| Host/Windows quirk | windows-phone-link-search-safety or frank-overlay | T0 / sanitized T1 |
| Multi-CLI routing | coding-agents | T4 + sanitized T1 |
| Single CLI flags | claude-code / codex / opencode | Official-aligned T1 |
| Completion discipline | todo-discipline | T1 core + T4 logs |
| Empire/strategy process | empire-planning | T4 |
| Awesome curation | awesome-list-maintenance | T1 process |
| Product packaging | skill-portfolio-ops + this OS | T4 process / T1 templates |
| Brand creative production | design-swarm / brand-image-system | T3 |
| Fitness N-of-1 | velora private instance | T4 / product T5 |

## Promote vs gate (after absorb)

```
Is the learning portable without Frank secrets?
  YES → sanitize → T1 free pack → public repo / hub
  NO  → does it power a paid SKU?
          YES → T3 vault / product docs
          NO  → T4 private only
```

## Self-evolution tooling (use, don’t wait)

| Tool | Role |
|------|------|
| `skill_manage(patch)` | Same-session improve |
| `hermes curator` | Lifecycle of agent-created skills |
| `skill-portfolio-ops` | Classification + promote gate |
| gencreator-swarm-evolver | Scheduled TEST/EVAL/EVOLVE cycles |
| multi-llm-arena | Measure agent/prompt quality |
| session_search | Mine past wins/failures |
| Optional: hermes-agent-self-evolution (DSPy/GEPA) | Evolve skill text when available |

## Weekly learning review (Queen / Frank)

1. session_search: “failure OR patch OR lesson OR pitfall”  
2. Diff skills touched this week  
3. Any skill patched ≥3 times → refactor (too much sediment)  
4. Any skill never loaded → archive candidate  
5. Promote queue: ship 1 free skill/pack per week minimum  

## Metrics that matter

| Metric | Target |
|--------|--------|
| Time-to-patch after failure | Same session |
| Free promotes / month | ≥4 high-quality |
| Orphan stubs (v0.1 no refs) | ↓ toward 0 |
| Description bloat (catalog) | Keep triggers short |
| Repeat user corrections | ↓ (memory + skills) |
| Public pack install health | CI green |

## Anti-patterns

- “We’ll write it up later” → lost learning  
- Patching only memory with procedures → wrong store (skills are procedures)  
- Promoting private failure logs with PII  
- Creating new skill instead of patching umbrella  
- Evolving skill text without verification checklist  

## Absorb log (append)

### 2026-07-15 — Skill Portfolio OS foundation

- Established dual-tree maintenance + T0–T5 classification  
- Rule: official leaves refreshable; Frank umbrellas local; free = sanitized  
- Self-learning mandatory session-end protocol  
- Products mapped open-core (not all-free, not all-gated)  
- Created `skill-portfolio-ops` Hermes skill + universe strategies package  

### 2026-07-15 — Wave 2 execution

- Absorbed MCR/AGY-MCR/SI into coding-agents; stubs are redirects  
- Free packs shipped; CSL PR #21; CoE kit SKU private outline  
- frank-overlay for claude-code leaf rebase  
- Funnel doc + weekly cron already scheduled  
- Learning: never push FrankX branches that inherited `.asph-wip` multi-100MB patches — branch from origin/main with pathspec commits only  

- 2026-08-03 — Weekly review: curator status still reported only `coding-agents` pinned after two local pin commands reported success; treat runtime-pin persistence as a T0/T4 operational verification item, not as a public-pack change.
- 2026-08-05 — Weekly review: curator again reported only `coding-agents` pinned while the registry requires five pins; retain this as a T0/T4 runtime-verification backlog, keep the three absorb-complete redirect stubs as documented aliases, and leave the sanitized Windows project-scoped search note as the active T1 promotion candidate.
- 2026-08-06 — Weekly review: curator still reports only `coding-agents` pinned (38 stale, none archived); public-pack scan found no redirect stubs, while the registry retains the three absorbed runtime aliases, so keep runtime-pin persistence as T0/T4 verification and the sanitized project-scoped-search note as the active T1 promotion candidate.
- 2026-08-10 — Weekly review: confirmed the three documented runtime redirects remain intentional; absorbed the duplicate `daily-building-in-public` surface into `build-in-public` as a T0 compatibility redirect, while the sanitized project-scoped-search note remains the active T1 promotion candidate.
- 2026-08-17 — Weekly review: curator reports 32 stale/0 archived and only `coding-agents` pinned; this cron also could not load its referenced bootstrap and path-safety skills. Classify pin/skill-registration verification as T0/T4 runtime work; retain the sanitized project-scoped-search note as the active T1 promotion candidate.
- 2026-08-28 — Weekly review: Hermes v0.20.6 is current; curator reports 2 managed agent-created skills with 0 stale/0 archived and 8 zero-activity unmanaged skills pending adoption review. No documented redirect stubs were found in active/public skill trees; the sanitized project-scoped-search note remains the active T1 promotion candidate, while missing runtime safety/process skills and pin-registration verification remain T0/T4 backlog.
