# Coding Rules

- Read the surrounding code and project-local instructions before editing.
- Prefer existing project conventions over new abstractions.
- Keep changes scoped to the user's request.
- Prefer the minimum code that solves the actual problem.
- Do not add speculative features, flexibility, configurability, or impossible-case handling.
- Do not rewrite unrelated code just because it could be nicer.
- Do not refactor adjacent code unless it is necessary for the task.
- Preserve user changes and do not revert work you did not make.
- Clean up only artifacts created by your own change, such as newly unused imports or variables.
- Every changed line should trace back to the user's request.
- Add comments only when they explain non-obvious intent.
- For non-trivial work, define success criteria before or during implementation.
- For bug fixes, prefer a reproducing test before the fix when practical.
- For refactors, verify behavior before and after when practical.
- Verify changes with the narrowest useful command, then broaden if risk warrants it.
- Use judgment for trivial tasks; do not add process ceremony when the answer is obvious.
- Put project-specific rules in the project repository, not this user-level workspace.
