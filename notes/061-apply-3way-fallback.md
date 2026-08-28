# Applying a patch that does not apply cleanly

The 3-way fallback uses blob metadata in the patch to merge instead of failing outright.

```bash
git apply --3way changes.patch
```
