# Human-readable version from tags

git describe yields tag+distance+sha, which is a perfect build identifier.

```bash
git describe --tags --always --dirty
```
