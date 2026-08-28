# Fetching just one branch

A narrow refspec avoids downloading refs you will never look at.

```bash
git fetch origin main:refs/remotes/origin/main
```
