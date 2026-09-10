# Agent Workspace

This workspace contains project context and references to code and requirements.

## Workspace structure

- `Projects/` — project context and boundaries.
- `Repositories.md` — repository roles and local paths.
- `Sources.md` — sources for requirements, contracts, and behavior.

Choose relevant projects, repositories, and sources based on the user's task. Load only the context needed.

## Working rules

- Read the target repository's local instructions before changing code.
- Verify changing details in source code.
- Report contradictions instead of guessing.
- Run the target package tests after edits.
- Keep requirements, typed representation, and app behavior in the owners identified by `Sources.md`.
