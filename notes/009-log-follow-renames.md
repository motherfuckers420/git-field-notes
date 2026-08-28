# Following a file across renames

Without --follow, history stops at the rename. With it, git tracks the file through its former names.

```bash
git log --follow -- path/to/file.ts
```
