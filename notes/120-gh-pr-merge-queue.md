# Merge queues keep main green

A queue re-tests each PR against the latest main before it lands, which prevents semantic conflicts.

```bash
gh api repos/{o}/{r}/rulesets
```
