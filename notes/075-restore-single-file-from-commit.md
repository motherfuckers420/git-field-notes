# Restoring one file from an old commit

restore --source pulls a single path out of history without touching anything else.

```bash
git restore --source=v1.2.0 -- src/config.ts
```
