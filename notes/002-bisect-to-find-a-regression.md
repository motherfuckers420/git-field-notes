# Binary-searching history for a regression

Bisect turns "somewhere in 400 commits" into ~9 checkouts. Give it a script and it runs unattended.

```bash
git bisect start HEAD v1.2.0 && git bisect run ./test.sh
```
