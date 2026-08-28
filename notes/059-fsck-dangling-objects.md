# Finding orphaned objects

fsck lists dangling commits and blobs, which is the last resort when reflog has been pruned.

```bash
git fsck --lost-found
```
