# Prefer switch and restore over checkout

checkout is overloaded. switch changes branches, restore changes files. Fewer catastrophic typos.

```bash
git switch -c feature && git restore --source=HEAD~1 file.ts
```
