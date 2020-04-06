== Minimal usage ==

```
  cd 10
  docker build -t postgres-pgaudit:10 .
  docker run \
    -e IS_AUDIT_LOG_ENABLED=true \
    -e PGAUDIT_LOG=ALL \
    -d --rm \
    postgres-pgaudit:10
```
