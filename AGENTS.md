# Agent Workspace: Feed Demo

This workspace routes agents to a small synthetic feed project. Do not search other folders under `Developer`.

## Routing

Aliases select the context needed for a request; they do not require every request to load a project note first. A route may point to repository mappings in `Repositories.md`, a large feature or initiative in `Projects/`, or requirements, findings, and progress in `Tasks/`. Add those notes and their routes only when needed; this minimal demo has no project notes; task notes are created only when needed.

| Request aliases | Context to read |
| --- | --- |
| “лента”, “выдача”, “feed”, “карточка”, card analytics, `ios-feed-app`, `analytics-contracts` | `Repositories.md` |

For the feed route:

1. Resolve exact repository paths and responsibilities through `Repositories.md`.
2. Read the relevant repository's `AGENTS.md` before changing code.
3. Read `Sources.md` to choose the authoritative source for the detail you need.
4. Verify the contract, implementation, and tests relevant to the request.

## Working rules

- Treat all context as synthetic demo data.
- Verify changing details in source code.
- Report contradictions instead of guessing.
- Run the target package tests after edits.
- Do not modify analytics contracts unless the task explicitly changes the schema.
