# Stashing new files too

Plain git stash leaves untracked files behind, which breaks builds in confusing ways.

```bash
git stash push -u -m "wip: parser"
```
