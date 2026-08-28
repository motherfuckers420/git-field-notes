# The dubious ownership error

git refuses to operate on repos owned by another user unless you mark them safe.

```bash
git config --global --add safe.directory /srv/app
```
