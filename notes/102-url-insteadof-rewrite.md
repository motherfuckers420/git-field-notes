# Rewriting remote URLs globally

insteadOf swaps HTTPS for SSH for every remote matching a prefix.

```bash
git config --global url."git@github.com:".insteadOf "https://github.com/"
```
