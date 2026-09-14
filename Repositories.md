# Repositories

All paths are intentionally exact. Do not substitute similarly named repositories.

| Alias | Purpose | Path |
| --- | --- | --- |
| `ios-feed-app` | Feed UI behavior and tests | `/Users/dimitrykodryan/Developer/feed-demo-repositories/ios-feed-app` |
| `analytics-contracts` | Canonical typed analytics event schemas | `/Users/dimitrykodryan/Developer/feed-demo-repositories/analytics-contracts` |

## Feed scope and repository relationships

The feed (лента, выдача) displays cards returned by a loader. Card analytics belongs to the feed domain.

- iOS behavior and feature changes belong in `ios-feed-app`.
- Canonical event schema: `analytics-contracts`. Event names and parameter schemas belong in this repository.
- For the card-tap task, inspect both repositories but make the feature change in `ios-feed-app`.
- Client-side tap handling is the demo scope. No backend or external system is in scope.
