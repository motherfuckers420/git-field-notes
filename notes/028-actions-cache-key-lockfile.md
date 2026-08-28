# Key your cache on the lockfile

Hashing the lockfile makes the cache invalidate exactly when dependencies change.

```bash
key: ${{ runner.os }}-node-${{ hashFiles('**/package-lock.json') }}
```
