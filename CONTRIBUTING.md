# Contributing

This is a **web-first** awesome list of other people's skills. FrankX packs belong last, labeled optional.

## Inclusion bar

A new entry needs all of:

1. A primary URL (GitHub preferred) with a real `SKILL.md` or documented install path.
2. One sentence of **distinct** value (not “awesome AI skill”).
3. License posture (SPDX or “read LICENSE”).
4. A review state: `reviewed`, `watch`, `unverified`, or `unsafe`.
5. A safety note if the skill can spend, post, delete, or exfiltrate.

Do **not** submit:

- Affiliate funnels, Gumroad CTAs, or “53 skills free if you RT”
- Unsigned ZIP / S3 skill blobs
- Wallet / broadcast-tx packs without a dry-run and human spend gate
- Duplicate canonical URLs
- Invented projects
- Bulk dumps (“add these 400 skills”)

## Earned-skill rule

Prefer packs operators actually run (one named job, readable source, recent maintenance). See [docs/EARNED-SKILLS.md](./docs/EARNED-SKILLS.md), [docs/QUALITY-AND-SAFETY.md](./docs/QUALITY-AND-SAFETY.md), and the always-do [docs/LIST-CONTRACT.md](./docs/LIST-CONTRACT.md).

Changing the core 5–7 start set requires a matching edit to [docs/earned.json](./docs/earned.json) in the same PR.

## How to submit

1. Fork and branch from `main`.
2. Add the row next to similar entries. Keep third-party work above FrankX packs.
3. Open a PR with the primary URL, why it belongs, license, and review state.

Agent / UI / deploy entries belong in [awesome-hermes-agents](https://github.com/frankxai/awesome-hermes-agents).
