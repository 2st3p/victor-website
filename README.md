# Victor Website

Personal website for Victor Donahue - built with Astro + Tailwind.

## Repository Structure

```
Victor Website/
├── site/              # Astro project (main application)
│   ├── src/          # Source files (pages, layouts, components, data)
│   ├── public/       # Static assets (images)
│   └── dist/         # Build output (generated, gitignored)
├── Backup images/    # Archive images (gitignored)
└── Image picks/      # Archive images (gitignored)
```

## Local Development

```bash
cd site
npm install
npm run dev
```

Visit `http://localhost:4321` to preview.

## Building

```bash
cd site
npm run build
npm run preview  # Preview the built site locally
```

Build output goes to `site/dist/`.

## Deployment (Cloudflare Pages)

The site is deployed to **victordonahue.com** via Cloudflare Pages.

### Repository
- **GitHub**: https://github.com/2st3p/victor-website
- **Production branch**: `main`

### Cloudflare Pages Settings

- **Framework preset**: Astro
- **Build command**: `cd site && npm install && npm run build`
- **Build output directory**: `site/dist`
- **Production branch**: `main`

### Custom Domain
- **Domain**: victordonahue.com
- Configured in Cloudflare Pages → Custom domains

### Auto-Deploy
Every push to `main` automatically triggers a new deployment.

## Updating Content

### Live Dates
Edit `site/src/data/live-dates.json`

### DJ Performances
Edit `site/src/data/dj-performances.json`

### Studio Tools
Edit `site/src/data/studio-tools.json`

### Site Links (Email, Socials, etc.)
Edit `site/src/data/site-links.json`

### Images
Replace files in `site/public/assets/`:
- `hero.jpg` - Hero section image
- `live-1.jpg`, `live-2.jpg` - Live performance images
- `studio.jpg` - Studio section image
- `dj.jpg` - DJ section image

Keep filenames the same to avoid code changes.

## Features

- **STROBE mode**: Top-right button rapidly inverts page colors (press `Esc` to stop)
- **Contact form**: Falls back to `mailto:` if no endpoint configured
- **Responsive design**: Built with Tailwind CSS

## Tech Stack

- [Astro](https://astro.build/) - Static site generator
- [Tailwind CSS](https://tailwindcss.com/) - Styling
- [Cloudflare Pages](https://pages.cloudflare.com/) - Hosting & CDN
