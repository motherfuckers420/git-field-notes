# Skipping untestable commits during bisect

Commits that do not build should be skipped, not marked good or bad.

```bash
git bisect skip
```
