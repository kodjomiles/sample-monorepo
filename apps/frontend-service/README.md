# Frontend Service

> Source: sample-monorepo / apps/frontend-service/README.md

React web application providing the user interface.

## Development

```bash
cd apps/frontend-service
npm install
npm run dev
```

## Build

```bash
npm run build
```

Production assets are output to `dist/`.

## Environment Variables

| Variable         | Description            |
|------------------|------------------------|
| `VITE_API_URL`   | Backend API base URL   |
| `VITE_AUTH_URL`  | OAuth provider URL     |

## Testing

Run unit tests with `npm test` and E2E tests with `npm run e2e`.
