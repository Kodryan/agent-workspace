# Feed Demo

The feed (лента, выдача) displays cards returned by a loader. Card analytics belongs to the feed domain.

Scope:

- iOS behavior: `ios-feed-app`
- Canonical event schema: `analytics-contracts`
- Feature changes belong in the app; event names and parameter schemas belong in contracts.
- The current request concerns client-side tap handling. No backend or external system is in scope.
