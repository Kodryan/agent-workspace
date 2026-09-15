# Repositories

Use these exact paths; do not substitute similarly named repositories.

| Repository | Path |
| --- | --- |
| `ios-feed-app` | `/Users/kodryan/Developer/demo/repositories/ios-feed-app` |
| `analytics-contracts` | `/Users/kodryan/Developer/demo/repositories/analytics-contracts` |

## Feed scope

Feed (лента, выдача) displays loader-returned cards; card analytics belongs to feed.

`ios-feed-app` owns UI behavior, features, and tests. `analytics-contracts` owns canonical event names and parameter schemas.
 For card tap, inspect both; change client-side handling in `ios-feed-app`. Backend and external systems are out of scope.
