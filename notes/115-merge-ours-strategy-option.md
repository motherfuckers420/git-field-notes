# Resolving a conflicted merge in favour of one side

-X ours only applies to conflicting hunks, unlike the -s ours strategy which discards the other side entirely.

```bash
git merge -X ours feature
```
