# Non-cone patterns for odd layouts

Non-cone mode accepts gitignore-style patterns when the cone model is too coarse.

```bash
git sparse-checkout set --no-cone '/*' '!/docs'
```
