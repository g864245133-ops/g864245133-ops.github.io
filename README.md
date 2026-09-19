# Xiaoyue Gao Academic Portfolio

This repository contains the initial framework for a personal academic website built with Astro.

## Core concepts

- **Page:** A file in `src/pages/` becomes a URL on the website.
- **Component:** A reusable interface fragment, such as the header or a content card.
- **Layout:** The shared HTML structure wrapped around individual pages.
- **Static site:** The final website is generated as HTML files before deployment.

## Run locally

Open this folder in Visual Studio Code, then open **Terminal → New Terminal** and run:

```bash
npm install
npm run dev
```

Open the local address printed in the terminal, usually `http://localhost:4321`.

## Build and preview

```bash
npm run build
npm run preview
```

`npm run build` creates the deployable site in `dist/`. Do not edit `dist/` directly; edit files in `src/` instead.

## Project map

- `src/pages/`: one file per website page
- `src/components/`: reusable interface pieces
- `src/layouts/`: shared page structure
- `src/styles/global.css`: visual design and responsive rules
- `src/data/site.ts`: name, affiliation, contact details, and navigation
- `public/`: files copied directly to the final site

## Current scope

This is intentionally an initial framework. It contains the full navigation and representative CV-based content, while leaving clear placeholders for a biography, profile image, AI projects, science communication, downloadable CV, GitHub, Google Scholar, ORCID, and LinkedIn.

## Deployment

The repository is configured for the GitHub user site `g864245133-ops.github.io`.
Every push to the `main` branch runs `.github/workflows/deploy.yml`, which builds the Astro project and publishes the generated site through GitHub Pages.
