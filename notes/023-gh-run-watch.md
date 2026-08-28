# Watch a workflow run to completion

gh run watch streams job status and exits non-zero on failure, so it composes in scripts.

```bash
gh run watch --exit-status
```
