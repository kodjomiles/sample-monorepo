# Backend Service Runbook

> Source: sample-monorepo / apps/backend-service/docs/runbook.md

Operational procedures for the backend service.

## Health Checks

- **Liveness**: `GET /health/live` returns 200 when the process is running.
- **Readiness**: `GET /health/ready` returns 200 when database connections are established.

## Common Alerts

### High Error Rate

1. Check application logs: `kubectl logs -l app=backend-service`.
2. Verify database connectivity.
3. Roll back recent deployments if error rate correlates with release.

### Memory Pressure

1. Review heap snapshots in Datadog APM.
2. Scale horizontally if traffic has increased.
3. Investigate memory leaks in recent PRs.

## Escalation

Page the on-call engineer via PagerDuty if issues persist beyond 15 minutes.
