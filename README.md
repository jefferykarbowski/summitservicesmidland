# Summit Services — Marketing Site

Single-page marketing site for **Summit Services**, a window washing and lawn care business serving the Tri-Cities of Michigan (Midland, Bay City, Saginaw).

Owners: Oliver Karbowski & Jackson Larson

## Stack

- [Astro 5](https://astro.build/) (static SSG)
- [Tailwind CSS v4](https://tailwindcss.com/) (CSS-first config via `@theme`)
- [Cloudflare Pages](https://pages.cloudflare.com/) (hosting + CDN)

## Local development

```sh
npm install
npm run dev      # http://localhost:4321
npm run build    # production build → dist/
npm run preview  # serve dist/ locally
```

## Project layout

```
src/
  layouts/Base.astro    # HTML shell, head, fonts, JSON-LD
  pages/index.astro     # Single-page site (all sections inline)
  pages/404.astro       # Not-found page
  styles/global.css     # Tailwind import + brand theme tokens
public/
  images/               # Logo, team photo, banner, social QR codes
  robots.txt
assets-source/          # Original image archive (not served)
```

## Deployment

Pushes to `main` auto-deploy to Cloudflare Pages.

- Project name: `summitservicesmidland`
- Production: https://summitservicesmidland.pages.dev (and `midlandsummitservices.com` once registered)
- Build command: `npm run build`
- Output directory: `dist`

PRs run typecheck + build via GitHub Actions.

## Brand

- Navy: `--color-navy-800` (#0d2b58)
- Sky: `--color-sky-bright` (#2c8ef0)
- Accent yellow: `--color-accent-400` (#facc15)
- Grass: `--color-grass-600` (#3f8a35)
