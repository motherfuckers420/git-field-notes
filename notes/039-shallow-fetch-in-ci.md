# Shallow fetch in CI, but mind the depth

depth 1 is fastest, but breaks anything that walks history, including some changelog tools.

```bash
git fetch --depth=1 origin main
```
