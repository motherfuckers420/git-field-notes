# Triggering a workflow manually

workflow_dispatch inputs can be passed from the CLI, which beats clicking through the UI.

```bash
gh workflow run deploy.yml -f environment=staging
```
