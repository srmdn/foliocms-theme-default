# Changelog

## v0.2.0 (2026-04-06)

API-driven content and settings.

- **Content from API**: switched from local filesystem content collections to fetching posts from the FolioCMS API at request time; no static content dir required in the theme
- **Settings from API**: site name and description are now read from `GET /api/settings`; configure them from the FolioCMS admin dashboard
- **Astro 6**: upgraded from Astro 5 to Astro 6 and `@astrojs/node@10`
- **Package manager**: switched from Bun to npm for broader compatibility
- Renamed project references from Inkwell to FolioCMS throughout

---

## v0.1.0 (2026-03-27)

First release.

- Astro SSR theme with post list, single post, and 404 pages
- Content read from local filesystem via Astro content collections
- Ships with FolioCMS installer by default

---

Releases follow [Semantic Versioning](https://semver.org).
