# Changelog

## v0.2.2 (2026-10-23)

Security patch.

- **Security**: upgraded Astro `6.1.1` to `7.4.2` and `@astrojs/node` `10.0.4` to `11.1.9`, resolving a critical XSS advisory in `define:vars` plus cache-poisoning and transitive dependency advisories; `npm audit` now reports 0 vulnerabilities
- **Astro 7**: adopted the Rust compiler, Vite 8, and the new default `compressHTML: 'jsx'`; rendered output was compared against v0.2.1 and matches apart from expected whitespace and CSS serialization differences
- **Verification**: `astro check` 0 errors, production build succeeds, standalone server returns 200 for home and post pages and 404 for unknown routes

---

## v0.2.1 (2026-04-06)

- **Fix**: hero image is now fetched from the API response and displayed at the top of the post page
- **Fix**: social links (GitHub, Twitter, LinkedIn) from site settings are now shown in the footer
- **Fix**: `/media/` path correctly proxied to the backend in reference nginx config

---

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
