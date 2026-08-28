# Check out only part of a monorepo

Sparse checkout limits the working tree to the paths you name, while history stays complete.

```bash
git sparse-checkout set apps/web packages/ui
```
