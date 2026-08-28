# Cancel superseded workflow runs

A concurrency group keyed on the ref cancels the previous run when you push again.

```bash
concurrency: {group: "${{ github.ref }}", cancel-in-progress: true}
```
