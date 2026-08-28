# Which commits are not upstream yet

git cherry marks commits with a plus when the upstream branch lacks an equivalent patch.

```bash
git cherry -v main feature
```
