---
name: coding-agents-superpack
description: "Use when orchestrating multiple coding agent CLIs (Claude Code, Codex, OpenCode, Grok CLI, Antigravity). Discovery, comparison, structured prompting, and multi-agent handoff patterns. Portable free pack — no host-specific secrets."
version: 1.0.0
author: Frank Riemer / GenCreator
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [Coding-Agent, Orchestration, Multi-CLI, Prompting, Free-Pack]
    related_skills: [claude-code, codex, opencode]
    provenance: frankx-public
    tier: free
---

# Coding Agents Superpack (Free)

Portable multi-CLI orchestration patterns for Hermes, Claude Code, Codex, OpenCode, Grok CLI, and similar agents.

**This free pack is sanitized.** Personal host quirks, private brand wiring, and machine-specific topology live in private overlays — not here.

## When to Use

- Multiple coding CLIs available; need discovery or comparison
- Designing structured prompts for autonomous coding agents
- Multi-agent collaboration with a shared board (Model Council pattern)
- Building hybrid “orchestrator drives + specialist CLI executes” workflows

**Don't use for:** single-CLI deep flags (load that vendor’s skill/docs); private multi-brand empire ops.

## Discovery (run first)

```bash
which codex && codex --version
which claude && claude --version && claude auth status
which opencode && opencode --version
which grok && grok --version
# health
codex doctor 2>/dev/null
claude doctor 2>/dev/null
```

Prefer **project-scoped** filesystem checks. Avoid recursive search from home or drive roots (slow, noisy, and unsafe on multi-device Windows setups).

Test agents in an isolated temp git repo:

```bash
TEST_DIR=$(mktemp -d)
cd "$TEST_DIR" && git init -q && echo "# test" > README.md && git add . && git commit -q -m init
```

## Headless modes (automation)

| Agent | Preferred non-interactive |
|-------|---------------------------|
| Claude Code | `claude -p "…" --max-turns N --allowedTools "Read,Edit,Bash"` |
| Codex | `codex exec "…"` (sandbox flags per install) |
| OpenCode | `opencode run "…"` |
| Grok CLI | `grok --always-approve "…"` (confirm flags for your version) |

## Universal prompt structure

```text
# Objective
Clear goal + measurable success criteria

# Context
1. Read these exact files first: …
2. Constraints: …

# Procedure
1. …
2. …

# Required Artifacts
- Files with exact paths
- Verification report

# Verification
Run tests/lint; report failures; do not claim done without evidence
```

## Model Council (lightweight multi-agent)

When agents must collaborate (not isolated one-shots):

1. Shared board file: `KANBAN_BOARD.md` (or Hermes kanban)
2. Shared state: `STATE.json` or equivalent
3. Role prompts force: **read board first**, **update board last**
4. Explicit handoff artifacts (`IMPLEMENTATION_BRIEF.md`, etc.)

Roles example: Chair · Planner · Implementer · Reviewer · Researcher

## Hybrid execution pattern

For large multi-repo work:

1. **Orchestrator** creates foundations with direct file/git ops (visible, fast)
2. **CLI specialists** get scoped tasks with `--max-turns` / budgets
3. Publish a single **execution report** that separates *done* vs *delegated queue*
4. Never leave silent open tasks without a handoff document

## Safety & cost

- Cap turns/budget on headless runs  
- Restrict tools to what the task needs  
- Prefer print/one-shot modes for CI  
- Clean up tmux/sessions after interactive work  
- Never put secrets in prompts or board files  

## Verification checklist

- [ ] Discovery run; versions recorded  
- [ ] Prompt includes Objective/Context/Procedure/Verification  
- [ ] Headless flags set (max-turns/tools)  
- [ ] Artifacts exist on disk; tests/lint reported  
- [ ] Board updated if multi-agent  

## Related free resources

- GenCreator / Starlight public OS repos on frankxai  
- Official Hermes skills: `claude-code`, `codex`, `opencode`, `hermes-agent`  
- Workflow Tier plugin (MIT multi-agent workflows)  

## License

MIT — Frank Riemer / GenCreator. Upstream CLI behavior belongs to their vendors.
