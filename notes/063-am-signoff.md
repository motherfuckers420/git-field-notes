# Applying mailbox patches with a signoff

git am replays patches as commits and can add the Signed-off-by trailer as it goes.

```bash
git am --signoff < patches.mbox
```
