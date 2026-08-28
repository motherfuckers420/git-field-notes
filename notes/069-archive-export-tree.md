# Exporting a tree without .git

git archive writes a tarball of any tree-ish, which is what you want for release artifacts.

```bash
git archive --format=tar.gz -o site.tgz HEAD
```
