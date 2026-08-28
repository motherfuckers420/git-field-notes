# Pushing several refs all-or-nothing

--atomic means either every ref updates or none do, which matters for tag plus branch releases.

```bash
git push --atomic origin main v1.4.0
```
