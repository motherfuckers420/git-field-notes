# Different identities per directory

includeIf switches your email and signing key based on the repo path, so work and personal stay separate.

```bash
[includeIf "gitdir:~/work/"] path = ~/.gitconfig-work
```
