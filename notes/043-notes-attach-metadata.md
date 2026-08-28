# Attach metadata to commits without rewriting

git notes stores data alongside a commit, so annotations do not change the SHA.

```bash
git notes add -m "verified in staging" <sha>
```
