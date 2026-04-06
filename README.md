# foliocms-theme-default

Default Astro SSR theme for [FolioCMS](https://github.com/srmdn/foliocms).

Clean, minimal blog frontend. Fetches posts and settings from the FolioCMS API at request time.
Ships with FolioCMS out of the box.

## Requirements

- Node.js 22+
- A running FolioCMS backend

## Setup

```bash
npm install
cp .env.example .env
# Edit .env: set BACKEND_URL to your FolioCMS backend address
npm run build
```

## Configuration

| Variable | Default | Description |
|----------|---------|-------------|
| `BACKEND_URL` | `http://localhost:8090` | Base URL of the FolioCMS backend API |

Site name and description are read from the FolioCMS settings API (`GET /api/settings`).
Configure them in the FolioCMS admin dashboard.

## Running after build

```bash
node dist/server/entry.mjs
```

Set `HOST` and `PORT` environment variables to control the server address.

## Building a custom theme

See [theme contract](https://github.com/srmdn/foliocms/blob/main/docs/theme-contract.md)
for the full specification.

## License

MIT
