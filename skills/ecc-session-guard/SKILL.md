---
name: ecc-session-guard
description: "Use when a Hermes session is about to edit a linter config or a TypeScript file. Warns on console.log and blocks weakening an existing formatter config. Does not install the ECC marketplace."
version: 1.0.0
author: Frank Riemer
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [hooks, config, console, ecc, guard]
    related_skills: [todo-discipline]
    provenance: upstream-ecc-mit
    tier: free
---

# ECC session guard

Two small hooks from [affaan-m/ECC](https://github.com/affaan-m/ECC) at `4eb71d92a39cab44ad40ac9d8a6a5ccb4029d6c2` (MIT, copyright 2026 Affaan Mustafa). The scripts live in `upstream-hooks/`. This page is the estate wrapper. It is not a bulk install of ECC.

## When to use

- An agent is editing ESLint, Prettier, Biome, Ruff, Stylelint, markdownlint, or `lint-ratchet-baseline.json` that already exists.
- An agent is editing `.ts`, `.tsx`, `.js`, or `.jsx` and may leave `console.log` behind.

Do not use this to install ECC profiles, a second orchestrator, or a memory store.

## What the scripts do

1. `upstream-hooks/config-protection.py` blocks an edit only when that config file already exists. Creating a new config is allowed. The hook fails open and writes a one-line diagnostic on stderr.
2. `upstream-hooks/check-console-log.py` warns on stderr and exits 0. Tests and scripts are excluded. It never blocks the edit.

## Estate limits

- Do not point config protection at `settings.json`. Frank has to be able to edit his own settings.
- Do not treat a markdown handover as a lint file.
- Review state for the upstream repo is `watch`. Browse named pieces. Do not copy the `full` profile into `~/.hermes`.

## Install

Copy this folder to `~/.hermes/skills/ecc-session-guard/` and wire the two scripts only if you want them in `~/.hermes/config.yaml`. Read `docs/HERMES-HOOKS.md` upstream before enabling a block.

## License

The Python files stay under the upstream MIT notice. This SKILL.md is MIT, Frank Riemer, and names the upstream commit above.
