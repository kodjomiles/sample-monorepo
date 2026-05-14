# Sample Monorepo

> Source: sample-monorepo / README.md

A reference monorepo demonstrating how Port ingests documentation from multiple services within a single repository.

## Repository Structure

```
apps/
  backend-service/     # Node.js API server
    docs/
      runbook.md       # Operational runbook
      architecture.md  # System design
  frontend-service/    # React web application
```

## Getting Started

```bash
npm install
npm run dev
```

## Documentation

Each service maintains its own `docs/` folder. Port's TechDocs integration ingests these as separate `techDoc` entities, scoped to the relevant service via the repository relation.
