# Query the GitHub API from the shell

gh api speaks REST and GraphQL and has jq built in, so you rarely need curl and a token.

```bash
gh api repos/{owner}/{repo}/pulls --jq '.[] | .number'
```
