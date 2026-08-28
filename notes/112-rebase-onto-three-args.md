# Moving a branch to a different base

rebase --onto replays only the commits between two points, which is how you fix a branch based on the wrong parent.

```bash
git rebase --onto main old-base feature
```
