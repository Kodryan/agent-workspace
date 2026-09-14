# Feed demo workspace

Routing-only workspace for the synthetic task “Залогировать нажатие карточки на выдаче”. Start with `AGENTS.md`.

The editable demo code lives in `/Users/dimitrykodryan/Developer/feed-demo-repositories`; this repository stores only context and routing. Use `Tasks/` only when a task needs persistent progress notes.

`AGENTS.md` maps request aliases to the context needed for the task. Feed aliases lead directly to `Repositories.md`, which records repository paths, responsibilities, and the canonical event-schema repository. `Sources.md` defines how to verify details.

Use `Projects/` for large features or initiatives and `Tasks/` for requirements, findings, and progress when needed. Their aliases can route directly to those notes; they are not mandatory steps before opening a repository. Project notes are not needed for this minimal feed demo; task notes remain optional.
