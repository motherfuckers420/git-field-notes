# Machine-readable commit trailers

Trailers are key/value lines git can parse, which is how Co-authored-by and Signed-off-by work.

```bash
git interpret-trailers --parse < .git/COMMIT_EDITMSG
```
