# Batch ref updates atomically

update-ref --stdin applies many ref changes in one transaction, all or nothing.

```bash
git update-ref --stdin < refs.txt
```
