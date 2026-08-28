# Require a linear history

Blocking merge commits on the default branch keeps bisect and revert predictable.

```bash
gh api -X PUT repos/{o}/{r}/branches/main/protection/required_linear_history
```
