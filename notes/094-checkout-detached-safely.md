# Working in detached HEAD without losing work

Commits made in detached HEAD are only reachable from the reflog until you name them.

```bash
git switch -c keep-this
```
