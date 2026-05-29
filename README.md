# harness-space

`harness-space` is a minimal user-level harness workspace for AI agents.

Its job is to give different AI tools a shared starting point before they work with the user or enter a project repository. It answers a few global questions:

- Who is the user?
- What voice and working temperament should the agent use?
- Which local projects exist, and where are they?
- What durable rules should agents follow across projects?

This repo is intentionally thin. It is not a project management system, a task tracker, a memory dump, or a copy of each project's docs. Project-specific context belongs inside the project repository.

## Files

- `SOUL.md` - the agent's durable voice, taste, and working temperament.
- `ME.md` - stable context about the user and their preferences.
- `PROJECTS.md` - a name-to-path index for local projects.
- `rules/` - durable user-level behavior rules for agents.
- `AGENTS.md` - adapter for Codex / OpenAI-style agents.
- `CLAUDE.md` - adapter for Claude Code-style agents.

## How Agents Should Use This

1. Read the relevant adapter file for the current tool, such as `AGENTS.md` or `CLAUDE.md`.
2. Load `SOUL.md`, `ME.md`, `PROJECTS.md`, and task-relevant files under `rules/`.
3. If the task targets a project, use `PROJECTS.md` only to find the path.
4. After entering that project, follow the project's own local instructions as the source of truth.

## Boundary

Keep this workspace small. Add only stable user-level context here:

- user preferences,
- global agent rules,
- project names and paths,
- tool adapters.

Do not add project status, todos, architecture notes, commands, ports, secrets, or task plans here.
