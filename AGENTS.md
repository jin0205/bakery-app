# Bakery app working agreement

## Automatic cross-computer continuity

The user authorizes routine commits and pushes of relevant project work to this repository. They do not need to announce a start or finish. Apply these steps to each task that changes files, not to ordinary conversation.

### Before editing
- Read HANDOFF.md and inspect the current branch, working tree, and upstream.
- Fetch origin. With a clean working tree, fast-forward the current branch from its matching upstream; never pull a different branch into it automatically.
- Preserve existing uncommitted work. Do not reset, clean, force-push, or silently stash it. If it prevents safe synchronization, explain the conflict before editing overlapping files.
- Follow the branch and next action recorded in HANDOFF.md. Use one active computer at a time; concurrent tasks need separate branches.

### Before a normal final response after changes
- Run checks appropriate to the change. Record actual results, including skipped or failing checks.
- Update HANDOFF.md with current branch, completed and unfinished work, checks, and the next action. Avoid recursive commit hashes in this file.
- Review the diff and stage only relevant files by name. Never commit secrets, dependencies, caches, or unrelated work.
- Commit and push the current branch, setting its upstream if needed. Verify the remote branch SHA matches the local commit. A successful local commit alone is not a successful sync.
- Report any push failure and retain the local commit for retry. Do not overwrite remote work to make a push succeed.

### Incomplete work
- When stopping normally with incomplete changes, preserve a clearly labeled WIP checkpoint on a work branch and push it. Keep its status and failing checks explicit in HANDOFF.md.
- Do not publish unfinished work to main merely to back it up. Before switching branches, preserve unrelated work and confirm no other task shares the checkout.
- These instructions cannot run after a crash, forced interruption, or power loss. No scheduled backup is configured by this file.

## Product decisions
- All product and piece weights mean dough weight before baking.
- Target dough grams = piece count × dough grams per piece. No finished-weight mode or bake-loss adjustment.
- Existing Bake, EZ-baker, and BakeryOS projects are reference material; leave them unchanged.
- The production preview is sample-data design work, not a production app or an approved final design.

## Portability
- Use repository-relative paths in scripts and handoffs. Keep machine paths and credentials out of shared configuration.
- Install dependencies separately on each computer. Commit the package-manager lockfile once a framework is chosen.
