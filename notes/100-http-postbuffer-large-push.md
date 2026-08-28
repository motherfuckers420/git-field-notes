# Large pushes failing over HTTPS

Raising the post buffer fixes the classic "RPC failed; curl 55" on big initial pushes.

```bash
git config http.postBuffer 524288000
```
