# Agent Workspace

This workspace is my personal routing map for coding agents. Keep stable project context here and verify changing implementation details in the current code.

## Routing

If a task relates to checkout or payments:

1. Read `Projects/Checkout.md`.
2. Resolve repository names and aliases through `Repositories.md`.
3. Use `Sources.md` when the task requires documentation or external systems.
4. Read the relevant repository-level `AGENTS.md` before changing code.


- Report contradictions between documentation and code instead of silently choosing one.
- Do not store secrets, tokens, or credentials in this workspace.
- For work that spans repositories or sessions, create or update `Tasks/<id>.md` from `Tasks/_template.md`.
- Add platform conventions only when a real task creates that need.
