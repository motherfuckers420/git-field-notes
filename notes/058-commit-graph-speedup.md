# Speed up history traversal

The commit-graph file caches commit metadata and makes log and merge-base much faster.

```bash
git commit-graph write --reachable
```
