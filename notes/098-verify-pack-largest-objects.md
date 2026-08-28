# Finding what makes a repo huge

verify-pack plus sort shows the largest objects, which is how you find the accidental 400MB video.

```bash
git verify-pack -v .git/objects/pack/*.idx | sort -k3 -n | tail
```
