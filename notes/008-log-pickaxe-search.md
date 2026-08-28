# Finding when a string was introduced

The pickaxe searches diffs, not file contents, so it finds the commit that added or removed a token.

```bash
git log -S "DEPRECATED_FLAG" --oneline
```
