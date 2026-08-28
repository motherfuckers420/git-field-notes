# Posting a long PR comment from a file

Passing a file avoids shell quoting problems with markdown and code fences.

```bash
gh pr comment 1234 --body-file review.md
```
