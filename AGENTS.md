# Agent Workspace: Feed Demo

This workspace routes agents to a small synthetic feed project. Do not search other folders under `Developer`.

## Routing

For requests containing “лента”, “выдача”, “feed”, “карточка”, or card analytics:

1. Read `Projects/Feed.md`.
2. Resolve exact repository paths through `Repositories.md`.
3. Read `Sources.md` to choose the authoritative source for the detail you need.
4. Read the target repository's `AGENTS.md` before changing code.

## Working rules

- Treat all context as synthetic demo data.
- Verify changing details in source code.
- Report contradictions instead of guessing.
- Run the target package tests after edits.
- Do not modify analytics contracts unless the task explicitly changes the schema.
