# Use worktrees instead of stashing

A worktree is a second checkout sharing one object store. Review a PR without disturbing your dirty tree.

```bash
git worktree add ../review-pr origin/feature-x
```
