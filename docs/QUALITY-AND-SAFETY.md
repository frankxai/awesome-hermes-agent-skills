# Skill quality and safety gate

This list is a **discovery surface**, not an install-everything marketplace. Stars, likes, and “awesome” badges are popularity signals. They are not safety proofs.

Review state used in this estate:

| State | Meaning | Allowed claim |
| --- | --- | --- |
| `reviewed` | Public README + license + listing URL checked on the pulse date. **Not** an independent SKILL.md audit unless `validation/evidence/` exists | Describe purpose |
| `watch` | Interesting; not a default install | “Emerging” |
| `unverified` | Seen on GitHub/search/X | Discovery only |
| `tested` | Named version run in a sandbox with stored evidence | “Tested on …” |
| `unsafe` | Failed heuristics or known malice | Do not recommend |
| `archived` | Historical | History only |

Nothing in a public README is `tested` unless `validation/evidence/` exists for that exact commit.

## Earned-skill doctrine

High-signal operators keep **about 5–7 skills they actually invoke**, not hundreds of unread packs.

Install a skill only when:

1. It does **one nameable job**.
2. You can **read the source** before it runs.
3. It has a **license** you accept.
4. It has been **updated in the last 90 days**, or it is a vendor-maintained official pack.
5. It does not need secrets, wallets, or production credentials to be useful.

Bulk catalogs (1,000+ skills, “all 53 free if you RT”, unsigned ZIP drops) are **directories**. Do not copy them into a live agent profile.

## Before you install

1. Open the primary GitHub repo. Confirm a real `SKILL.md` (or documented install path).
2. Read the skill body for hidden instructions: fetch URLs, write to `~`, dump env, disable approvals, “ignore previous”.
3. Check license. `NOASSERTION` means read `LICENSE` yourself.
4. Prefer official vendor packs and small operator methodologies over anonymous dumps.
5. Scan with [NVIDIA SkillSpector](https://github.com/NVIDIA/SkillSpector) (Apache-2.0). Docs: [scanning agent skills](https://docs.nvidia.com/skills/scanning-agent-skills). A clean score is a signal, not a warranty.
6. Install into a **throwaway profile / worktree**, not the business agent, until you trust it.

## Default quarantine

Do **not** recommend or auto-install:

- OpenClaw / ClawHub dumps and unsigned `skill.md` site lists
- Wallet, signing, staking, or broadcast-transaction skills unless the operator has a dry-run path and a human spend gate
- Remote ZIP / S3 skill blobs with no repo, no license, and no pinned commit
- Prompt-injection / malware-in-`SKILL.md` reports (Huntress FakeAgent-style campaigns)
- “Install our 300–2,000 skills” control planes as a second operating system — ACOS, Superpowers, and gstack already cover that job if you need a methodology

## Human gates (always)

Keep human approval on: production deploys, public posts, money movement, DNS, credentials, legal/IP, destructive data ops, and history rewrites.

## Provenance for this pulse

GitHub repository metadata and X public posts were sampled on **2026-08-30**. Star counts are that day’s discovery snapshot. Primary README and license remain authoritative.
