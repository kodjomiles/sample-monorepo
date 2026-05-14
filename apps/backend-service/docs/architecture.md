# Backend Service Architecture

> Source: sample-monorepo / apps/backend-service/docs/architecture.md

## Overview

The backend service follows a layered architecture:

```
+----------------+
|   Controllers  |   HTTP request handling
+----------------+
        |
+----------------+
|    Services    |   Business logic
+----------------+
        |
+----------------+
|  Repositories  |   Data access
+----------------+
        |
+----------------+
|   PostgreSQL   |   Persistence
+----------------+
```

## Key Decisions

1. **Express.js** chosen for its ecosystem maturity.
2. **TypeORM** for database migrations and queries.
3. **Redis** for session caching and rate limiting.

## Dependencies

- PostgreSQL 14+
- Redis 7+
- Node.js 20 LTS
