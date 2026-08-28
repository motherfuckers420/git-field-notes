# Aggressive gc is rarely worth it

It repacks everything and can take hours. Normal gc plus maintenance is almost always enough.

```bash
git gc --prune=now
```
