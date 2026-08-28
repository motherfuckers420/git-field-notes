# Purging a secret from history

filter-repo rewrites history. The leaked credential is still compromised, so rotate it first.

```bash
git filter-repo --invert-paths --path config/secrets.yml
```
