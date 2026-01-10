# Victor Website
Static single-page site built with Astro + Tailwind.

Top-right `STROBE` button rapidly inverts the page colors (images unchanged). Press `Esc` to stop.

## Local dev

```sh
cd "Desktop/Victor Website/site"
npm install
npm run dev
```

Build static output to `dist/`:

```sh
npm run build
npm run preview
```

## Update content (JSON-driven)

Edit these files:

- `src/data/live-dates.json` — live dates list
- `src/data/dj-performances.json` — selected performances list
- `src/data/studio-tools.json` — studio tools list
- `src/data/site-links.json` — emails + socials + DJ mix link

## Update images

Replace files in `public/assets/` (keep filenames the same to avoid touching layout code):

- `public/assets/hero.jpg`
- `public/assets/live-1.jpg`
- `public/assets/live-2.jpg`
- `public/assets/studio.jpg`
- `public/assets/dj.jpg`

## Contact form

Default behavior: if no endpoint is configured, the form falls back to a `mailto:` compose to `hello@victor.com`.

To enable a hosted form provider, set `src/data/site-links.json`:

- `contactForm.endpoint`: e.g. `https://formspree.io/f/YOUR_FORM_ID` (or Basin/Getform/etc)

## Deploy (Cloudflare Pages)

Project root: `site/`

- Build command: `npm run build`
- Build output directory: `dist`
