# foliocms-theme-default

Default Astro SSR theme for [FolioCMS](https://github.com/srmdn/foliocms).

Clean, minimal blog frontend. Reads Markdown posts from the filesystem.
Ships with FolioCMS out of the box.

## Requirements

- Node.js 22+
- A FolioCMS backend with posts in `CONTENT_DIR`

## Setup

```bash
npm install
cp .env.example .env
# Edit .env: set CONTENT_DIR to your FolioCMS content path
npm run build
```

## Configuration

| Variable | Default | Description |
|----------|---------|-------------|
| `CONTENT_DIR` | `../content/blog` | Path to FolioCMS's content directory |
| `SITE_NAME` | `My Blog` | Site name shown in the header and page titles |
| `SITE_DESCRIPTION` | _(empty)_ | Meta description for the home page |

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
