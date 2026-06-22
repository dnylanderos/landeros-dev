# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```sh
pnpm dev        # Start dev server at localhost:4321
pnpm build      # Build production site to ./dist/
pnpm preview    # Preview production build locally
pnpm astro add  # Add integrations (e.g. tailwind, react, mdx)
```

## Architecture

This is an [Astro](https://astro.build) site using the **basics** starter template, running Astro v6 with strict TypeScript.

- `src/pages/` — file-based routing; each `.astro` file becomes a URL
- `src/layouts/` — reusable page shells (currently `Layout.astro` wraps all pages with the base HTML)
- `src/components/` — UI components consumed by pages and layouts
- `src/assets/` — static assets processed/optimized by Astro's build pipeline
- `public/` — files served verbatim at the root URL (favicons, robots.txt, etc.)

Pages compose layouts and components using Astro's frontmatter fence (`---`) for server-side logic and the template body for markup. No JS framework is configured yet; adding one (React, Svelte, etc.) requires `pnpm astro add <integration>`.

Package management uses **pnpm** (workspace configured in `pnpm-workspace.yaml`). Node ≥ 22.12.0 required.
