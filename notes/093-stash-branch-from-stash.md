# Turning a stash into a branch

If the stash no longer applies, stash branch checks out the original commit first.

```bash
git stash branch fix/parser stash@{2}
```
