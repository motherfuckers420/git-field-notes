# Fixup commits that rebase themselves

Commit with --fixup and the interactive rebase pre-orders and marks it. No manual reordering.

```bash
git commit --fixup=<sha> && git rebase -i --autosquash <sha>~1
```
