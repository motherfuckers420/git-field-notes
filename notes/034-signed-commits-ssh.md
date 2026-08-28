# Sign commits with your SSH key

Since git 2.34 you can sign with SSH, so no GPG keyring to maintain.

```bash
git config gpg.format ssh && git config user.signingkey ~/.ssh/id_ed25519.pub
```
