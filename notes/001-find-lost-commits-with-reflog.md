# Recovering commits after a bad reset

`git reset --hard` does not delete commits, it moves a pointer. Every position HEAD has held is in the reflog for 90 days.

```bash
git reflog --date=iso | head -30 && git branch rescue <sha>
```
