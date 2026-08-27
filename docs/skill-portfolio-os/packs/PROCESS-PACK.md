# Process pack (Approach A)

**Status:** recipe shipped in git · skills.sh pack URL **pending founder Vercel create**  
**Updated:** 2026-08-27  
**SKU:** free T1 composition (not a new GitHub repo)

One job: give any coding harness the **minimum process stack** — todos match reality, multi-CLI orchestration, then Superpowers TDD/debug/brainstorm. Five skills. No MCP required.

## Why this is a pack, not another repo

- Listed marketplace units already exist: `npx skills add frankxai/skills` (Architect) and `npx skills add frankxai/creator-skills` (Creator).
- skills.sh **packs** are unlisted URL bundles. Anyone with the link can install. Not access-controlled.
- This repo already contains exactly two SKILL.md trees (`todo-discipline`, `coding-agents-superpack`). Attaching the whole repo to a pack includes those two only — do not attach Hermes runtime or awesome-* catalogs.

## Contents (5)

| Skill | Source | Why |
| --- | --- | --- |
| `todo-discipline` | this repo `skills/todo-discipline` | completion gate |
| `coding-agents-superpack` | this repo `skills/coding-agents-superpack` | multi-CLI, sanitized |
| `brainstorming` | `obra/superpowers` (public) | design before build |
| `test-driven-development` | `obra/superpowers` (public) | red-green |
| `systematic-debugging` | `obra/superpowers` (public) | root-cause before patch |

**MCP pair:** none. Process skills are when/how to think. Do not bundle Railway, Stripe, or creator MCP credentials.

**Hard excludes:** Hermes `%LOCALAPPDATA%/hermes/skills` dump, Phone Link / host T0, profiles, empire/CoE, any awesome-* catalog, `starlight-creator-mcp` packs (different schema).

## Install (until the unlisted pack URL exists)

GitHub (this repo — two FrankX skills):

```sh
npx skills add frankxai/awesome-hermes-agent-skills --skill todo-discipline --skill coding-agents-superpack
```

Superpowers (three public skills):

```sh
npx skills add obra/superpowers --skill brainstorming --skill test-driven-development --skill systematic-debugging
```

Hermes (copy folders; this CLI does not target Hermes):

```sh
git clone https://github.com/frankxai/awesome-hermes-agent-skills.git
cp -R awesome-hermes-agent-skills/skills/todo-discipline ~/.hermes/skills/
cp -R awesome-hermes-agent-skills/skills/coding-agents-superpack ~/.hermes/skills/
```

When the skills.sh pack exists:

```sh
npx skills add https://skills.sh/p/<pack-id>
```

Paste the id into `PACK-URL.md` in this folder (gitignored if it must stay unlisted-but-known; otherwise record in FUNNEL.md).

## Create on skills.sh (founder click)

Packs are owned by a Vercel team. Sign-in is human-gated.

1. Open https://skills.sh/packs/create and sign in with Vercel.
2. Name: `frankx-process` (or `Process`). Description: `Todo discipline + coding-agents superpack + Superpowers brainstorm/TDD/debug. Five skills. No MCP.`
3. Team: the FrankX/Starlight Vercel team already used for frankx.ai (do **not** create a new Vercel project).
4. Add sources:
   - GitHub `frankxai/awesome-hermes-agent-skills` (yields the two SKILL.md in `skills/`)
   - Public skills: `brainstorming`, `test-driven-development`, `systematic-debugging` from obra/superpowers
5. Create. Copy `npx skills add https://skills.sh/p/<id>`.
6. Record the id here / FUNNEL.md. Do not put secrets in the pack. Delete the pack to kill the link.

Telemetry: `npx skills` sends anonymous skill-name telemetry unless `DISABLE_TELEMETRY=1`.

## Related listed units (do not duplicate)

| Unit | Command | MCP pair |
| --- | --- | --- |
| Architect | `npx skills add frankxai/skills` | context7 |
| Creator | `npx skills add frankxai/creator-skills` | `starlight-creator-mcp` when npm-published |
| Process | this pack | none |

`creator-pack-manifest.v1` (MCP brand data) is **not** a skills.sh pack. Do not mix schemas.
