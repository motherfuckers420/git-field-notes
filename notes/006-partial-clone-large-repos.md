# Cloning huge repos without the history

A blobless clone fetches file contents on demand. Minutes become seconds on large monorepos.

```bash
git clone --filter=blob:none <url>
```
