# cron-as-a-service
A cron application where users can define a job and a schedule for it to run on.

## Infrastructure

A PostgreSQL server is provided via Docker. Use `docker-compose` from the
`infrastructure` directory to start it:

```bash
cd infrastructure
docker-compose up -d
```

The server listens on port `5432` and uses the following default credentials:
- **user**: `cron`
- **password**: `cronpass`
- **database**: `cron_db`
