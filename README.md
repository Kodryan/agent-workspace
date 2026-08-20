# Agent Workspace

A personal Markdown workspace that helps coding agents find the right project context, repositories, and external sources.

## Structure

- `AGENTS.md` — routes requests to relevant context.
- `Projects/` — personal context about projects and their boundaries.
- `Tasks/` — optional task notes for work that spans repositories or sessions.
- `Repositories.md` — repository URLs, local working copies, aliases, roles, and relationships.
- `Sources.md` — guidance for choosing Jira, documentation, code, contracts, and runtime sources.

## Context flow

```text
User request or ticket
└── AGENTS.md                       router
    ├── Projects/<Project>.md       personal project context
    │   └── Repositories.md         aliases, locations, relationships
    │       └── Repository
    │           ├── AGENTS.md       repository rules
    │           └── Current code    implementation source of truth
    ├── Sources.md                  Jira, docs, contracts, runtime data
    └── Tasks/<id>.md               spec and working state, when needed
```

## Access

Markdown does not grant filesystem access. Add repository directories when starting the agent, for example with `codex -C <workspace> --add-dir <repo>` or `claude --add-dir <repo>`. In an existing session, the agent may request permission for a specific operation, but the workspace cannot expand the sandbox by itself.
