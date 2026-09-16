# Agent Workspace

This workspace is my personal routing map for coding agents. Keep stable project context here and verify changing implementation details in the current code.

## Routing

Aliases select relevant context; there is no mandatory project-first sequence. Load only the notes needed for the request.

| Request aliases                                                                                                                     | Context to read        |
| ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------- |
| `ios-app`, `app`, `main-app`, `payments-package`, `payments`, `checkout-contracts`, `contracts`, `checkout-backend`, `checkout-api` | `Repositories.md`      |
| checkout initiative                                                                                                                 | `Projects/Checkout.md` |

- Add aliases for features, initiatives, and task notes when those notes are created. Aliases may point directly to `Projects/<name>.md` or `Tasks/<id>.md`.
- Resolve repository locations and relationships through `Repositories.md` when code is needed.
- Read the target repository's `AGENTS.md` before changing code.
- Use `Sources.md` when a claim needs verification in documentation, contracts, or external systems.
- Use `Projects/` for lasting context about large features or initiatives and `Tasks/` for requirements, findings, decisions, and progress of a specific task.

## Working rules

- Report contradictions between documentation and code instead of silently choosing one.
- Do not store secrets, tokens, or credentials in this workspace.
- For work that spans repositories or sessions, create or update `Tasks/<id>.md` from `Tasks/_template.md`.
- Add platform conventions only when a real task creates that need.
