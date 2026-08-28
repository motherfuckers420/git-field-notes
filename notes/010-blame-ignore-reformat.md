# Blame that skips the big reformat

Record bulk-formatting commits in a file and blame will look straight through them.

```bash
git blame --ignore-revs-file .git-blame-ignore-revs file.ts
```
