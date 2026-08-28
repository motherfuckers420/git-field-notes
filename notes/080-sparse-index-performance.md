# Sparse index for very large checkouts

The sparse index keeps the index proportional to your cone, not the whole repo.

```bash
git sparse-checkout init --cone --sparse-index
```
