# Windows Project-Scoped Search Note (T1 Draft)

**Status:** Sanitized public draft — 2026-09-14
**Purpose:** A portable filesystem-discovery practice for Windows users who work across multiple repositories, synced folders, removable media, or device integrations.

## Default rule

Start every recursive search at the smallest verified project directory that can contain the answer. Do not begin at a drive root or at the user-profile root.

This is a reliability rule, not just a performance preference: broad scans are slow, collect unrelated private material, make results harder to audit, and can trigger unwanted access in multi-device environments.

## Safe workflow

1. Identify the repository or workspace that owns the question.
2. Verify its root with the version-control tool before searching or editing.
3. Constrain searches to a named subdirectory where possible (for example, `src/`, `docs/`, or `skills/`).
4. Prefer filename and content filters to unbounded recursive scans.
5. If the project root is unknown, inspect the workspace map, repository list, or remote metadata first; do not widen the search to a personal home directory.
6. Before reporting completion, state the exact searched root and verify that no broader root was used.

## Portable examples

```bash
# Work from a verified repository root.
cd C:/work/acme-app
git rev-parse --show-toplevel

# Search only the source tree for one precise symbol.
rg -n --glob '*.ts' 'createSession' src/

# Locate a known documentation file within this repository only.
rg --files docs | rg 'DEPLOYMENT\.md$'
```

## Boundaries

- Do not present this note as a replacement for an organization's incident-specific host-safety procedure.
- Do not publish personal paths, device names, sync-provider details, or incident logs in examples.
- When a task genuinely spans multiple repositories, enumerate the approved roots and search each one separately.

## Verification checklist

- [ ] Every recursive command has an explicit project or subdirectory root.
- [ ] The repository root was verified before any write.
- [ ] No drive-root or user-profile-root recursive search was used.
- [ ] Examples are portable and contain no personal identifiers or credentials.

## Promotion gate

This note is a T1 candidate only after the standard sanitizer checklist passes and it is linked from a public discoverability surface.
