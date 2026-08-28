# Cherry-picking a range of commits

The A..B range excludes A. Use A~1..B when you want A included.

```bash
git cherry-pick main~4..main~1
```
