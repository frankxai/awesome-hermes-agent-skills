# Weekly Skill Ops Checklist

- [ ] Explicitly set `$HERMES_HOME` to the target profile, echo it, then run `hermes curator status` and `hermes curator run --dry-run`; record the profile scope and do not trust an inherited scheduled-job environment
- [ ] Pins present (path-safety, todo-discipline, coding-agents, hermes-agent, skill-portfolio-ops)
- [ ] Verify pin flags in `$HERMES_HOME/skills/.usage.json`; `curator status` does not show them. Pin only eligible installed skills, and record absent or bundled exceptions as runtime remediation.
- [ ] Review curator-managed agent-created skills; archive only a named dry-run-proposed transition (the reported candidate count is the evaluated pool, not archive eligibility).
- [ ] Diff official leaves if Hermes updated; re-apply overlays
- [ ] Absorb ≥1 learning into a skill, checklist, or reference patch
- [ ] Advance promote queue (≥1 free pack in progress)
- [ ] Update TIER-REGISTRY if tiers changed
- [ ] Verify registry candidate/stub paths in the active profile before reporting their installed state; only exact evidence can confirm a redirect/absorb, while missing or full legacy pages remain T0/T4 migration work
- [ ] For a present legacy page, record its SHA-256 and canonical comparator; exact-path inspection alone determines redirect versus full-copy status
- [ ] No broad user-profile or drive-root recursive searches ran on Frank host this week
