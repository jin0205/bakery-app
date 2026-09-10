# Bakery app handoff

Updated: 2026-09-09
Branch: main

## Current state
- Shared GitHub repository: jin0205/bakery-app.
- Mac checkout created at the user's Codex projects location.
- Cross-computer working instructions added in AGENTS.md.
- Cross-platform line endings and initial ignore rules added.
- Windows checkout and two-way synchronization verification are pending.

## Product progress
- Prior task produced a fresh-start brief, project inventory, V1 scope, and interactive production preview. These remain in that task's outputs; this initialization does not silently migrate them.
- A previous document transfer to Windows was dispatched, but its results were not visible from the Mac. Preserve any existing Windows documents.
- Confirmed: every piece weight is dough weight before baking.
- Next product step: review the production preview before application implementation.

## Verification
- GitHub repository was empty before initialization.
- Documentation-only setup; no application tests apply.

## Next action
Complete the Windows checkout without overwriting existing files, verify it receives this main commit, then push a handoff update from Windows and fast-forward it on Mac. Record the verified outcome here.

## Limits
No timed backup, crash recovery service, or automatic operating-system file synchronization has been installed. AGENTS.md instructs task-level checkpoints; it is not a background service.
