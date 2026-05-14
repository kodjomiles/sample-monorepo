# Backend Service

> Source: sample-monorepo / apps/backend-service/README.md

Node.js API server providing REST endpoints for the platform.

## Quick Start

```bash
cd apps/backend-service
npm install
npm run start
```

## Environment Variables

| Variable       | Description              | Default     |
|----------------|--------------------------|-------------|
| `PORT`         | HTTP listen port         | 3000        |
| `DATABASE_URL` | PostgreSQL connection    | (required)  |
| `LOG_LEVEL`    | Logging verbosity        | info        |

## API Reference

See `/docs/openapi.yaml` for the full OpenAPI specification.
