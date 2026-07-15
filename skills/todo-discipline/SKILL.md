---
name: todo-discipline
description: "Use when starting any complex task (3+ steps) or before declaring work complete. Enforces todo/task state to match reality — merge updates + read verification. Prevents false completion."
version: 1.0.0
author: Frank Riemer / GenCreator
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [todo, task-management, discipline, verification]
    related_skills: []
    provenance: frankx-public
    tier: free
---

# Todo Discipline (Free)

Agents often create task lists, do the work, then conclude while the UI still shows **0/N done**. This skill makes **task state = reality** a hard gate.

## When to Use

- Complex tasks with 3+ steps  
- Multi-agent or long sessions  
- Before any “done”, handover, or “battle-tested” claim  

**Don't use for:** single-step Q&A.

## Hard gate

Before any concluding message:

1. Update **every** finished item to completed (merge, don’t wipe history)  
2. **Immediately read** the task list again (no-args read)  
3. Only then write the final summary  

Treat the **read result** as ground truth if merge responses echo stale state (common in long/headless runs).

## Rules

- Prefer merge over full replace  
- Only one item `in_progress` at a time  
- Never pass an empty todos array on merge (can clear the list)  
- Supply full id + content + **new** status for items you change  

## Verification checklist

- [ ] All finished work marked completed  
- [ ] No stale in_progress when claiming done  
- [ ] Read-back confirmed  
- [ ] User-visible task counter matches reality  

## License

MIT — Frank Riemer / GenCreator.
