# Managing repository secrets

gh secret set reads from stdin so the value never lands in your shell history.

```bash
gh secret set NPM_TOKEN < token.txt
```
