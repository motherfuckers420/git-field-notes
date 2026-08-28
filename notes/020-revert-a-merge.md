# Reverting a merge commit

A merge has two parents, so revert needs -m to say which side to keep.

```bash
git revert -m 1 <merge-sha>
```
