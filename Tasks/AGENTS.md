# Task Notes

Task notes preserve personal working context for work that spans repositories or sessions.

## Creating a note

- Create a note only when the user asks for one or the work is likely to span repositories or sessions.
- Copy `_template.md` and name the note after the ticket or a short task name.
- Fill the spec from the user's request and linked primary sources. Mark missing information as unknown instead of inventing it.
- Treat the spec as the task boundary. Ask before materially expanding its scope.

## During work

- Keep the note concise and update it after meaningful findings or decisions.
- Link findings to code paths, tickets, documents, or other evidence.
- Record decisions separately from hypotheses and open questions.
- Keep `Next step` specific enough for another session to continue.
- Verify changing implementation details in current code.

## After work

- Record the final outcome and any remaining follow-up.
- Move stable project knowledge to `../Projects/` and repository relationships to `../Repositories.md`.
- Do not copy secrets, tokens, credentials, or large source excerpts into task notes.
