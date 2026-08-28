# Caching credentials safely

The cache helper keeps the token in memory for a bounded time instead of on disk.

```bash
git config --global credential.helper 'cache --timeout=3600'
```
