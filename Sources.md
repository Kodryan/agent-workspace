# Sources

Choose sources by the question being answered, not merely by tool availability.

## Source selection

- Jira: task intent, acceptance criteria, comments, links, and current status.
- Confluence: product agreements, analytical specifications, and maintained internal documentation.
- Code host: current code, pull requests, and change history.
- API contracts: actual wire payloads and schema compatibility.
- Service registry: backend ownership and service dependencies.
- Grafana or another observability system: production behavior and runtime metrics.

## Evidence rules

- Requirements for an analytics event: check Jira and the analytics specification.
- Actual wire payload: check the contract and current code.
- Production behavior: check observability data.
- Implementation details: verify against the user-specified revision or `main`; follow `Repositories.md` before switching a local checkout.
- When sources disagree, show the conflict and identify which claim each source supports.
