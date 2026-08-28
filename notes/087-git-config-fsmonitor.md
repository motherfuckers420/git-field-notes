# Speed up status on large trees

The filesystem monitor avoids a full scan on every status call.

```bash
git config core.fsmonitor true
```
