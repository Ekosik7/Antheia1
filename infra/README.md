# Infrastructure planning

Future local topology: React client, Go backend, PostgreSQL and an optional Python image service under Docker / Docker Compose. Go provides the application API. Database and image service should stay on a private service network.

No Dockerfile, Compose file, database initialization or deployment exists. Ports, health checks, volumes, backup/restore, TLS, retention and resource limits need later decisions. Kubernetes is outside the MVP.

See [decisions](../docs/architecture/decisions.md) and [proposed environment names](../.env.example).
