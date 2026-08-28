# Reading raw git objects

cat-file is the lowest-level way to see what git actually stored.

```bash
git cat-file -p HEAD^{tree}
```
