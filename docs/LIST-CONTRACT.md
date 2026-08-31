# List contract (always)

Copy this into every public `awesome-*` we ship. It is the product, not a style guide.

This list must beat a dump (0xNyk, VoltAgent, “53 skills free if you RT”) on **safety, start time, and honesty** — not on row count.

## First screen

1. Five to seven **named jobs**, not a catalog. Table: pack · job · review state.
2. One safety line: read `SKILL.md`, then scan with [NVIDIA SkillSpector](https://github.com/NVIDIA/SkillSpector) (`--no-llm` is enough to start).
3. The page stays useful if every `frankxai` link is removed.
4. No mermaid, no 6-Pillar, no Gumroad, no “THE definitive”.
5. Hero on first screen only if ≤150 KB. Unused `hero.jpg` is deleted.
6. `## License` matches the SPDX file (full grant text, not a stub).

## Review states (only these)

`reviewed` · `watch` · `unverified` · `unsafe`

Never write `tested` without `validation/evidence/` for that commit.

## Digital (supply chain)

- No live GitHub URL to a **private** repo (looks like a 404).
- No unsigned ZIP / S3 skill blob.
- No wallet / broadcast-tx without dry-run **and** a human spend cap.
- OpenClaw / ClawHub dumps are directories, never a default OS.
- `pull_request` lychee fails the PR. Monthly issue filing is extra, not instead.

## Critical (honesty)

- Stars are a dated discovery snapshot, not quality.
- Do not claim affiliation with Nous, NVIDIA, or Anthropic.
- Directories (0xNyk, VoltAgent, Composio, sickn33) are labeled **browse, do not bulk-install**.
- wondelai/skills is a library to pick **named** skills from — never “great first install”.

## Taste (adoption)

- Time-to-first-skill: [GETTING_STARTED.md](../GETTING_STARTED.md) is ninety seconds to **one** named pack.
- Agents load the same start set from [earned.json](./earned.json).
- FrankX packs last, optional, secret-free.
- CONTRIBUTING rejects dumps. One entry per PR.

## Human gates (always)

Production deploys, public posts, money, DNS, credentials, legal/IP, destructive data, history rewrite.
