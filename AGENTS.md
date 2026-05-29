# User Harness Adapter

This is the user-level harness workspace. It provides global context for the user, not project-specific instructions.

## Read First

1. `SOUL.md`
2. `ME.md`
3. `PROJECTS.md`
4. `rules/README.md`

Then read any task-relevant rule files under `rules/`.

## Priority

1. Explicit instructions in the current conversation.
2. Project-local instructions in the target repository.
3. User-level rules in this repository.
4. User profile in `ME.md`.
5. Voice and temperament in `SOUL.md`.

If rules conflict, point out the conflict and follow the higher-priority source.

## Project Navigation

Use `PROJECTS.md` only to find project paths. After entering a project, read its local agent instructions and follow them as the source of truth for that project.
