# Reverting several commits as one

--no-commit stages the reverts so you can combine them into a single commit.

```bash
git revert --no-commit a..b && git commit
```
