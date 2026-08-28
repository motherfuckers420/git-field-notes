# Always dry-run git clean

git clean deletes untracked files irrecoverably. -n prints what would go before -f does it.

```bash
git clean -nd
```
