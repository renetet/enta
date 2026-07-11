# ENTA AI Automation Website

Astro-based static website for `enta.at`, focused on AI automation services in Vienna and the wider EU market. The site is designed for GitHub Pages/static hosting and uses German as the default language with English support through the `lang` query parameter.

## Current Scope

- Professional marketing website for AI automation consulting
- German and English content via `src/config/i18n.json`
- Warm Austria/Vienna-inspired visual identity
- Static pages suitable for GitHub Pages
- Home hero slider with optimized WebP images
- Contact form markup prepared for a static form provider such as Web3Forms
- EU-focused positioning for AI automation, including preference for EU-hosted LLMs and EU-hosted/self-hosted workflow services

## Main Routes

- `/` - Home
- `/automation` - AI automation positioning and stack
- `/services` - Services
- `/pricing` - Pricing examples
- `/portfolio` - Project examples
- `/ressourcen` - German resources page
- `/free-resources` - English resources page
- `/kontakt` - German contact page
- `/contact` - English contact page
- `/privacy-policy` - Privacy policy
- `/impressum` - Imprint

Language is selected with:

```text
?lang=de
?lang=en
```

## Tech Stack

- Astro 5
- Tailwind CSS
- React Icons
- TypeScript
- Static image assets in `public/images`

## Development

Install dependencies:

```bash
npm install
```

Run the local dev server:

```bash
npm run dev
```

Build the static site:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

## Content

Most editable website copy is stored in:

```text
src/config/i18n.json
```

Navigation is configured in:

```text
src/config/menu.json
```

Global site settings are configured in:

```text
src/config/config.json
```

## Static Forms

The contact forms are static-hosting friendly. For GitHub Pages, a service such as Web3Forms can be used by adding an access key in the relevant contact form configuration/code. Until a production key is added, the form markup can be reviewed locally without requiring a backend.

## Asset Notes

The hero slider uses optimized WebP files:

```text
public/images/home-slider-planning.webp
public/images/home-slider-workflow.webp
public/images/home-slider-monitoring.webp
```

Generated PNG source files for those slider images are intentionally ignored because the WebP versions are the production assets.

## Deployment

The project outputs a static site to:

```text
dist/
```

This makes it suitable for GitHub Pages, Netlify, or any static host.
