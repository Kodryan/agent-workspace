# Agent Workspace

A personal Markdown workspace that helps coding agents find the right project context, repositories, and external sources.

## Structure

- `AGENTS.md` — routes requests to relevant context.
- `Projects/` — context about large features and initiatives, loaded when relevant.
- `Tasks/` — optional task notes for work that spans repositories or sessions.
- `Repositories.md` — repository URLs, local working copies, aliases, roles, and relationships.
- `Sources.md` — guidance for choosing Jira, documentation, code, contracts, and runtime sources.

## Context flow

```text
User request or ticket
└── AGENTS.md                       rules, aliases, routing
    ├── Repositories.md            repository locations and relationships
    │   └── Repository AGENTS.md   local rules before code changes
    ├── Projects/<name>.md         feature or initiative context, when relevant
    ├── Tasks/<id>.md              requirements, findings, and progress
    └── Sources.md                where to verify details, when needed
```

Choose branches according to the task; do not read every context file by default. Add routes when creating project or task notes.

## Access

Markdown does not grant filesystem access. Add repository directories when starting the agent, for example with `codex -C <workspace> --add-dir <repo>` or `claude --add-dir <repo>`. In an existing session, the agent may request permission for a specific operation, but the workspace cannot expand the sandbox by itself.
