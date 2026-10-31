# {{TITLE}}

A Fernhill Software product. Built from intent
[{{INTENT}}](https://github.com/nictuck/fernhill-platform/tree/main/intent/{{INTENT_DIR}}).

| | |
|---|---|
| Staging | set after first deploy |
| Production | set after first release |
| Process | [fernhill-platform/docs/flow.md](https://github.com/nictuck/fernhill-platform/blob/main/docs/flow.md) |

## Develop

```bash
make check      # build + test + lint, what CI runs
make build
make test
make lint
```

## Ship

Merge to `main` deploys **staging** automatically. **Production** waits for
the release manager to approve the `production` environment in Actions.
Rollback: see CLAUDE.md.
